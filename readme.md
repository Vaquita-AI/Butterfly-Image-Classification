# Butterfly Species Classification with ResNet50
 
## Overview
This project utilizes the ResNet50 architecture to classify butterfly species. The model is fine-tuned on a combined dataset of butterfly images and then split into training and testing sets programmatically, rather than using predefined folders.

## Data Sources
- AI Planet: [Butterfly Identification Challenge](https://aiplanet.com/challenges/325/butterfly_identification/data)
- Kaggle: [Butterfly Image Classification Dataset](https://www.kaggle.com/datasets/phucthaiv02/butterfly-image-classification)

## Project Structure
```plaintext
.
├── model/                               # Directory for the trained model and weights
├── butterfly_classification.ipynb       # Jupyter notebook with training scripts
└── README.md                            # Project documentation
```

## Dependencies
- Python 3.10
- TensorFlow 2.x
- Keras
- Pandas
- NumPy
- Matplotlib
- Pillow
To install the required dependencies, run:
```bash
pip install tensorflow keras pandas numpy matplotlib pillow
```

## Data Preparation
The original dataset combined into one folder and then programmatically split into training, validation, and testing sets using a custom script. This method allows for dynamic and reproducible partitioning of the data.

## Training the Model
The model was trained using the best hyperparameters obtained from hyperparameter tuning, which includes a batch size of 64, a learning rate of approximately 0.0001116, and unfreezing the top 30 layers of the model.

## Results
The fine-tuned model demonstrates strong performance on the test dataset, with detailed performance metrics available in the notebooks/ directory.

## Contributing
Contributions are welcome. Please fork the repository and submit a pull request with your suggested changes.

## License
This project is licensed under the Apache license 2.0 - see the LICENSE file for details
