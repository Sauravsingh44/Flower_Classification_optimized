# Flower Classifier Model

## Overview
This repository contains a machine learning project that classifies images of flowers into one of nine categories using a convolutional neural network (CNN). The model is built with TensorFlow and Keras, and it is trained to recognize the following flower species:

- Bougainvillea
- Daisy
- Dandelion
- Frangipani
- Hibiscus
- Rose
- Sunflower
- Tulips
- Zinnia

## Features
- **Model Architecture**: A CNN model trained for flower classification.
- **Image Preprocessing**: Images are resized to 150x150 pixels and normalized to enhance performance.
- **Prediction Functionality**: Predicts the flower species for a given image and displays the image with the predicted label and confidence score.

## Dependencies
- Python 
- TensorFlow 
- NumPy
- Matplotlib

## Usage
### Model Prediction
1. Clone the repository:
   ```bash
   https://github.com/Sauravsingh44/Flower_Classification_optimized.git
   ```
2. Place the saved model file (`flower_classifier_model.h5`) in the root directory of the project.
3. Run the prediction script:
   ```bash
   python predict_flower.py
   ```
4. Update the `image_path` variable in the script with the path to your image:
   ```python
   image_path = r"path_to_your_image.jpg"
   ```
5. The script will display the image along with the predicted class and confidence score.

### Example Output
```plaintext
Predicted Class: Sunflower with 100% confidence.
```
The image will also be displayed with the label and confidence score using Matplotlib.

## Code Structure
- `predict_flower.py`: Contains the code for loading the model, preprocessing the image, predicting the class, and displaying the result.
- `flower_classifier_model.h5`: Pre-trained model (not included; you must provide it).
- `requirements.txt`: List of required Python packages.

## How It Works
1. The input image is resized to 150x150 pixels and normalized to have values between 0 and 1.
2. The model predicts a probability distribution over the nine flower classes.
3. The class with the highest probability is selected as the predicted label.
4. The confidence score is displayed along with the predicted label.

## Customization
- **Adding Classes**: Update the `class_labels` list and retrain the model with new data.
- **Adjusting Image Dimensions**: Modify `img_height` and `img_width` parameters in the script to match your training dataset.

## Contribution
Contributions are welcome! Feel free to open an issue or submit a pull request for improvements, bug fixes, or new features.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments
- TensorFlow and Keras for providing excellent machine learning tools.
- The open-source community for datasets and inspiration.


