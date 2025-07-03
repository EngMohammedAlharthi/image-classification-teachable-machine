The predict.py script is used to run predictions on images using the trained model exported from Teachable Machine.

How the script works:
- By loading the model, The script loads the trained Keras model from the file keras_model.h5.

- Load class labels
It reads the class names (e.g., "Dallah Coffee Pot", "Date") from the file labels.txt.

- Load and preprocess the image
The input image is resized to 224x224 pixels and normalized to match the format the model was trained on.

- Run prediction
The image is passed into the model, and a prediction is made. The model returns confidence scores for each class.

- Display result
The class with the highest confidence is selected and printed along with its confidence score.
.
..

Test Results for Two Images:

Image 1: Dallah_CO.jpg
Description: Image of a traditional Arabic coffee pot (Dallah)

Expected class: Dallah Coffee Pot

Predicted class: Dallah Coffee Pot

Confidence score: 0.9997
.
..

Image 2: Date.jpg
Description: Image of a date fruit

Expected class: Date

Predicted class: Date

Confidence score: 0.9984
