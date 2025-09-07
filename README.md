# GeoAI for Sustainable Urban Development: AI-Powered Change Detection

### Project Overview
This project presents a novel **GeoAI (Geospatial Artificial Intelligence)** solution for monitoring urban development and environmental change. It leverages deep learning to automatically detect and classify land-use changes from satellite imagery, a task that is traditionally time-consuming and labor-intensive for urban planners and environmental agencies. The system provides a powerful, data-driven tool to track urbanization, deforestation, and infrastructure growth over time.

### Dataset
The model is trained on a synthetic dataset that simulates pairs of satellite images taken at two different time points (`t1` and `t2`). These image pairs are accompanied by a binary mask representing the areas of change. This synthetic approach allows for the demonstration of a complete end-to-end workflow, from data preparation to model inference. The underlying principles are directly applicable to public datasets such as Sentinel-2 or Landsat.

### Methodology
1.  **Data Generation and Preprocessing:** Synthetic satellite image pairs and their corresponding change masks are generated to represent land-use shifts. The data is then preprocessed by normalizing pixel values and ensuring images are in the correct format for the model.
2.  **Model Architecture (Semantic Segmentation):** A **U-Net** architecture is used for this task. U-Net is a type of convolutional neural network specifically designed for **semantic segmentation**, a computer vision technique that classifies each pixel in an image. Its unique encoder-decoder structure allows it to accurately identify the precise location and shape of the changes.
3.  **Training and Evaluation:** The U-Net model is trained to learn the relationship between the image pairs and the change masks. The model is evaluated on a validation set, with performance measured by key metrics like **Dice Loss** and **IoU (Intersection over Union)**, which are standard for segmentation tasks.
4.  **Inference and Visualization:** The trained model is used to predict changes on unseen image pairs. The results are visualized by overlaying the predicted change masks on the original images, providing a clear and intuitive representation of the detected urban expansion or environmental shifts.

### Concluded Results
The **GeoAI** model successfully identifies land-use changes with a high degree of accuracy, as validated by a strong IoU score. The project demonstrates the potential of AI to automate complex geospatial analysis, providing a scalable and efficient solution for monitoring urban growth and informing policy decisions. This project showcases advanced skills in computer vision, deep learning for segmentation, and a practical application of AI to solve a real-world societal problem.

### Technologies Used
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
