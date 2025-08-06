# Upcycle Website

A simple web application featuring AI chatbot and machine learning model to help generate upcycle ideas of piece of clothing. This repo consist of web dev and clothing dections classification.


## Technologies Used

- HTML5
- CSS3 (with Google Fonts and Boxicons)
- JavaScript (Vanilla)
- ResNet50

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/xainasx/upcycle-website.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd upcycle-website
   ```
3. **Open `index.html` in your browser.**

_No build steps or server needed; works as a static site._

## File Structure

- `Clothing dectection.ipynb` – Main Jupyter notebook containing all code.
- `index.html` – Main page with login and signup forms
- `style.css` – Styling for the forms and layout
- `script.js` – Handles password visibility toggle and form switching

## Customization

- Update social login button URLs to connect with your authentication providers.
- Adjust styles and layout in `style.css` as desired.

  The notebook walks through the following key steps:

1. **Data Loading and Exploration:**  
   - Loads image data and corresponding labels from CSV files.
   - Explores and visualizes dataset distributions.

2. **Data Preprocessing:**  
   - Cleans the dataset, removing corrupted images and unwanted label classes.
   - Performs exploratory data analysis and visualizations to understand class balance.

3. **Data Augmentation:**  
   - Applies augmentation techniques such as rotation, shifting, zooming, and flipping using `ImageDataGenerator` to improve model robustness.

4. **Model Building:**  
   - Uses the pre-trained ResNet50 model from TensorFlow/Keras as a feature extractor.
   - Customizes the top layers for the specific clothing classification task.
   - Fine-tunes the entire model for improved accuracy.

5. **Training and Validation:**  
   - Trains the model with early stopping and learning rate reduction callbacks.
   - Evaluates performance using accuracy and loss metrics.
   - Visualizes training curves.

6. **Prediction & Visualization:**  
   - Predicts on validation and unseen test images.
   - Visualizes predictions alongside true labels for qualitative assessment.

## Key Features

- **End-to-End Clothing Detection:** Includes data loading, cleaning, augmentation, model building, training, and prediction.
- **Transfer Learning:** Utilizes a powerful pre-trained ResNet50 architecture for feature extraction.
- **Visualization:** Offers rich visualizations for both data analysis and model predictions.
- **Easy Customization:** Can be adapted to different datasets or clothing categories by adjusting the CSV and image directory inputs.
## License

This project is for educational and research purposes. Please check the dataset and base model license for any usage restrictions.

---

**Repository:** [xainasx/upcycle-website](https://github.com/xainasx/upcycle-website)

