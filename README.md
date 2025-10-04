# FakeSniff - Open Source DeepFake Detection

FakeSniff is a Streamlit-based web application designed for detecting DeepFake content in images, videos, and audio files. It provides an intuitive interface for users to analyze media and determine its authenticity using advanced machine learning techniques.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)
- [License](#license)
- [Contact Information](#contact-information)

## Features

- **Multi-Model Detection**: Utilizes multiple DeepFake detection models to analyze media content:
  - `example_model_image.py`: Basic image deepfake detection model
  - `n_video.py` and `a_video.py`: Video deepfake detection models
  - Support for Hugging Face models integration
- **File Upload**: Supports uploading images (jpg, png, jpeg), videos (mp4, mov), and audio files (mp3, wav).
- **URL Input**: Allows users to input URLs for image, video, or audio analysis.
- **Processing Unit Selection**: Option to use GPU for supported models (default is CPU).
- **Result Visualization**:
  - Displays DeepFake detection statistics in a table format.
  - Provides downloadable CSV of detection results.
  - Visualizes results with bar charts for DeepFake probability and inference time.

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/akshay-jain-22/Speech-Detection.git
   cd Speech-Detection
   ```

2. **Create a conda environment**:

   ```bash
   conda create -n fakesniff python=3.8 -y
   conda activate fakesniff
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Model Setup**:

   The application includes several pre-configured models:
   - `example_model_image.py`: For image deepfake detection
   - `n_video.py` and `a_video.py`: For video deepfake detection
   - Hugging Face model integration support

   You can also add your own custom models by following the instructions in `Add_Custom_Model_to_DeepSafe.md`.

5. **Start the application**:

   ```bash
   streamlit run main.py
   ```

## Usage

1. **Select the "Detector" option** from the sidebar.
2. **Upload an image, video, or audio file**, or provide a URL.
3. **Choose one or multiple DeepFake detection models** you want to use.
4. **Optionally select GPU processing** if available.
5. **Click "Real or Fake? 🤔"** to start the analysis.
6. **View the results** in the displayed charts and tables, comparing outputs from different models.

## Future Work

FakeSniff aims to incorporate newer models and expand its capabilities to enhance DeepFake detection accuracy and efficiency.

## Contributing

We welcome contributions from the community. Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss the proposed changes.

## Acknowledgments

Developed by:
- Ashutosh Kumar Singh
- Sonu Patel
- Akshay Jain
- Gourav Aggraval

## License

This project is licensed under the MIT License.

## Contact Information

For inquiries or collaborations, please contact us through the GitHub repository.
