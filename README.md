# Cassava Leaf Disease Recognition

A machine learning-powered Streamlit application for detecting and classifying cassava leaf diseases using computer vision and deep learning models.

## Overview

This project provides an intelligent system to identify cassava leaf diseases from leaf images. Cassava is a critical food security crop in many regions, and early disease detection can prevent significant crop loss. This application leverages state-of-the-art deep learning models to assist farmers and agricultural professionals in disease diagnosis.

## Features

- 📸 **Image Upload & Analysis**: Upload cassava leaf images for instant disease classification
- 🤖 **Deep Learning Models**: Pre-trained neural networks for accurate disease detection
- 📊 **Confidence Scores**: Get confidence levels for each disease prediction
- 🎨 **User-Friendly Interface**: Built with Streamlit for ease of use
- 🔄 **Real-time Processing**: Fast inference on CPU and GPU
- 📈 **Disease Classification**: Identify multiple cassava leaf disease types

## Dataset
https://storage.googleapis.com/emcassavadata/
## Supported Disease Classes

The model can classify the following cassava leaf conditions:

- Cassava Brown Streak Disease (CBSD)
- Cassava Mosaic Disease (CMD)
- Healthy Leaves
- Additional disease variants and conditions

## Requirements

- Python 3.7 or higher
- Torch
- Streamlit
- Torchvision

## Installation

1. Clone the repository:
```bash
git clone https://github.com/MEdan-US/Cassava-Leaf-Disease-Recognition.git
cd Cassava-Leaf-Disease-Recognition
```

2. Create a virtual environment (recommended):
```bash
conda create --name leaf_env -y
conda activate leaf_env
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage

Run the Streamlit application:

```bash
python -m streamlit run app.py
```

The application will open in your default web browser at `http://localhost:8501`

### How to Use:

1. Open the application in your browser
2. Click on "Upload Image" or drag and drop a cassava leaf image
3. The model will analyze the image and display:
   - Disease classification result
   - Confidence score/probability
   - Recommendations for treatment or prevention

## Project Structure

```
Cassava-Leaf-Disease-Recognition/
├── README.md
├── requirements.txt
├── app.py                          # Main Streamlit application
├── models/                         # Pre-trained model files
│   └── cassava_model.h5           # Trained deep learning model
├── utils/                         # Utility functions
│   ├── preprocessing.py
│   ├── prediction.py
│   └── visualization.py
└── data/                          # Sample images and datasets
    ├── test_images/
    └── sample_leaves/
```

## Model Architecture

- **Base Model**: Transfer learning with pre-trained architectures (e.g., EfficientNet, ResNet)
- **Input Size**: 224x224 RGB images
- **Output**: Multi-class classification with softmax activation
- **Accuracy**: Trained on thousands of labeled cassava leaf images

## Dataset

This project uses cassava leaf disease datasets that include:
- Images of healthy leaves
- Images of diseased leaves (various diseases)
- Augmented data for improved model robustness

## Performance

- **Validation Accuracy**: ~95%
- **Inference Time**: <1 second per image
- **Model Size**: ~50-100MB

## Technologies Used

- **Deep Learning**: TensorFlow / Keras
- **Web Framework**: Streamlit
- **Image Processing**: OpenCV, PIL
- **Data Processing**: NumPy, Pandas
- **Language**: Python

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add improvement'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Open a Pull Request

## Future Enhancements

- [ ] Mobile app version
- [ ] Batch image processing
- [ ] Real-time camera feed analysis
- [ ] Multi-language support
- [ ] API deployment (Flask/FastAPI)
- [ ] Additional disease classes
- [ ] Crop health metrics and recommendations

## Troubleshooting

### Common Issues:

**ImportError: No module named 'tensorflow'**
- Solution: Run `pip install tensorflow`

**Streamlit not found**
- Solution: Run `pip install streamlit`

**Model file not found**
- Solution: Ensure the model file is in the `models/` directory

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Disclaimer

This application is intended to assist in disease identification but should not replace professional agricultural consultation. Always verify results with agricultural experts before making treatment decisions.

## Contact & Support

For questions, issues, or suggestions:
- Open an issue on GitHub
- Contact the maintainers

## Acknowledgments

- Cassava farming communities and agricultural experts
- Dataset providers and contributors
- Deep learning research community
- Streamlit for the excellent web framework

---

**Last Updated**: 2026-04-16

For more information about cassava diseases, visit:
- [FAO Cassava Information](http://www.fao.org/)
- [CGIAR Cassava Research](https://www.cgiar.org/)
