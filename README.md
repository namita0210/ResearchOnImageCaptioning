#Machine Learning Mastery Blog Tutorial
<a href="https://machinelearningmastery.com/develop-a-deep-learning-caption-generation-model-in-python/">Tap here to know more</a>
<li>extract_features(directory), that uses a pre-trained VGG16 model to extract features from images in a specified directory. It iterates through the images, preprocesses them to fit the VGG16 model, passes them through the model, and stores the extracted features in a dictionary with unique identifiers corresponding to each image. Finally, it saves the extracted features to a file named 'features.pkl'. <br>
so basically it consists of image features corresponding to image names which are reffered to as image identifiers.
That means this is a mathematical representation of images as matrices corresponding to their image identifiers.
</li>

<li>load_doc(filename) function:

Opens a file, reads its content, and returns the text from the file.
load_descriptions(doc) function:

Processes the text (presumed image descriptions) received as input.
Creates a dictionary where image identifiers are keys and associated descriptions are stored in lists.
Splits the text into lines, processes each line to extract image identifiers and descriptions, then stores them in the dictionary.</li>

<li>clean_descriptions(descriptions), takes a dictionary where image identifiers are keys and lists of descriptions are values. It performs text preprocessing on these descriptions by:

Lowercasing all words.
Removing punctuation, single-character words, and non-alphabetic characters.
Replacing the original descriptions in the dictionary with the cleaned versions.</li>

<li>save_descriptions(descriptions, filename), is intended to save processed image descriptions to a text file. It iterates through a dictionary where image identifiers are keys and lists of preprocessed descriptions are values. For each image identifier and its associated descriptions, it constructs a string combining the identifier and description. Then, it writes these combined strings, each on a separate line, to the specified file.</li>

<li></li>
