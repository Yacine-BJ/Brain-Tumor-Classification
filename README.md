# Brain-Tumor-Classification
This project focuses on automated brain tumor detection and classification from MRI images using the CRISP-DM data science methodology. The images are preprocessed by resizing them to 128×128 pixels, converting grayscale images into RGB format, and applying standardization to normalize pixel intensity distributions. Data augmentation techniques such as rotation, flipping, zooming, and translation are used to improve model robustness and generalization.

The detection model is built using Deep Learning, specifically Convolutional Neural Networks (CNNs) with transfer learning based on DenseNet121 pretrained on ImageNet. The convolutional layers are partially frozen while the final classification layers are fine-tuned to adapt to MRI-specific features. Training is performed using a reduced learning rate with regularization techniques to prevent overfitting.

The model is implemented using Python and scientific computing libraries such as NumPy and Pandas for data processing and manipulation. Performance evaluation shows 98% accuracy on internal validation data and 78% on external datasets, indicating some dataset distribution shift. The confusion matrix analysis shows that glioma tumors are more challenging to detect.

The trained model is deployed using Gradio, providing a simple web interface where users can upload MRI images, obtain tumor classification predictions, and view prediction confidence scores.

## Technologies used:

### Programming & Data Processing: Python, NumPy, Pandas

### Deep Learning: CNNs, Transfer Learning, DenseNet121

### Frameworks & Deployment: Gradio
