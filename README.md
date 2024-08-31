<h1 align='center'> Brain Tumor Detection </h1>
<p align='center'>Detecting Tumor in Brain MRI via Semantic Segmentation done with UNET.</p>
<p align='center'> 
The project leverages a custom-built U-Net architecture and popular pre-trained models, ResNet50 and VGG19_bn, using the `segmentation_models_pytorch` library. These models have been fine-tuned and adapted for the specific task of brain tumor segmentation. The dataset used in this project can be <a href='https://www.kaggle.com/datasets/pkdarabi/brain-tumor-image-dataset-semantic-segmentation/data'>found here</a>.
</p>

### Model Architectures

- **U-Net**: A custom-designed U-Net model was created specifically for this project, focusing on preserving fine-grained details in the segmentation process.
- **ResNet50**: A pre-trained ResNet50 model was utilized as an encoder within the U-Net architecture, allowing the model to benefit from the powerful feature extraction capabilities of ResNet50.
- **VGG19_bn**: Similarly, the VGG19_bn model was employed as an encoder, known for its deep feature extraction layers that are highly effective in image segmentation tasks.

### Model Selection

Various encoders were tested during the project, but ResNet50 and VGG19_bn emerged as the most effective for this specific task. Their ability to capture intricate details in medical images contributed to their superior performance.

### Evaluation Metrics

The models were evaluated using the following metrics:

- **Intersection over Union (IoU)**: IoU was used to measure the overlap between the predicted segmentation and the ground truth, providing a robust evaluation of model performance.
- **Mean Squared Error (MSE)**: MSE was employed to assess the difference between the predicted and actual segmentation masks, ensuring precision in the model's predictions.
