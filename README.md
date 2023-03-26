# Tomato detection using CNN
The tomato_detection_cnn.ipynb file is used to train a CNN model on the dataset in the tomato.zip file.

# Dataset
It's a .zip file containing images of tomato and images of grass and other images that are likely to be around tomatoes which are used for training the model to identify what is a tomato and what is not. These images have been extracted by the bing-image-downloader module which is used to download bulk of images from Bing.com.

# How to use bing-image-downloader to download images
Install bing-image-downloader using this command:
pip install bing-image-downloader

Then import the module and specify the query string, limit (maximum number of images to download) and output_dir which is the output directory (the directory of the local system where the images should be stored. Specify other parameters as preferred. 

from bing_image_downloader import downloader
downloader.download(query_string, limit=100,  output_dir='dataset', adult_filter_off=True, force_replace=False, timeout=60, verbose=True)

# The CNN model
Download tomato.zip and store it in My Drive on your Google drive.
Open tomato_detection_cnn.ipynb in colab and train the model. 
(Note: The last cell is used to test the model using random images with/ without tomato. You can use your own images to do this by having them in '/content/tomato/' in colab.)

# Conclusion
This project is an illustration of how CNN model can be trained using a custom dataset to detect tomatoes in an image. It could show better performance with a larger dataset.

# Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
