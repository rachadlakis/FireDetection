# Fire Detection Model

This repository contains the code and results for creating a Fire Detection model using binary image classification. The model is designed to predict whether an image contains fire or not. The process involves searching for the "best" model using Keras Tuner, considering both large and small model sizes.

## Use Cases

1. **Fire Emergency Response:**
   Implement the model in surveillance systems to detect fire occurrences and alert relevant authorities in real-time, enabling faster response and minimizing the impact of fire incidents on lives and property.

2. **Smart Home Safety:**
   Integrate the model into smart home systems for proactive fire monitoring. In case of a fire, homeowners receive immediate alerts for swift evacuation, and the system can trigger sprinkler systems to control the situation effectively.

3. **Forest Fire Monitoring:**
   Utilize drones equipped with the model to monitor forest areas for signs of fire, particularly in wildfire-prone regions. Real-time detection facilitates rapid firefighting measures, supporting environmental conservation efforts.

4. **Industrial Safety Compliance:**
   Deploy the model in industrial settings to monitor fire-related hazards, ensuring safety compliance and reducing the risk of workplace accidents associated with fire incidents.

5. **Insurance Claim Verification:**
   Insurers can employ the model to validate fire damage claims by comparing claimant-provided images with the model's fire identification. This assists in fraud detection and improves the accuracy of claim processing.

## Dataset Creation

The first step in building this Fire Detection model was creating the dataset. We combined multiple datasets of indoor and outdoor images, including fire and non-fire images:

- [Fire Dataset (755 outdoor-fire images)](https://www.kaggle.com/datasets/phylake1337/fire-dataset) (406 MB)
- [Forest Fire Dataset (950 fire images)](https://www.kaggle.com/datasets/alik05/forest-fire-dataset) (149 MB)
- [Fire Detection Dataset (110 fire images)](https://www.kaggle.com/datasets/atulyakumar98/test-dataset) (138 MB)
- Custom dataset: This dataset consisted of 494 fire images and 523 non-fire images. We generated non-fire images by searching for various keywords related to fire incidents, such as "Kitchen fire," "Electrical fire," and "Forest fire." Additionally, we included images of maple trees to help the model distinguish between the red color in trees and actual fire.

The combination of these datasets provided a diverse set of images for training and testing the Fire Detection model.

## Model Development

The model development process involved searching for the best architecture using Keras Tuner. We explored both large and small model sizes to find the optimal trade-off between accuracy and computational efficiency.

The code and results of this model development process are included in this repository, allowing you to replicate the experiments and create your own Fire Detection model.

Feel free to explore the code, experiment with different hyperparameters, and adapt the model for your specific use case. If you have any questions or suggestions, please don't hesitate to reach out. We hope this repository helps you in building effective fire detection solutions.
