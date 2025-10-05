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

    <br/>
   <h1><b>You can download models from here</b></h1>
  
   https://drive.google.com/drive/folders/1bdzx0TJELfHQ4dDtzeTFtTFMpO4U7I-O

6. **Start the application**:

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

<h2><b>Benchmarking</b></h2>
FakeSniff includes a powerful benchmarking feature that allows users to benchmark their datasets against selected deepfake detection models. The results include accuracy, precision, and recall metrics, along with detailed visualizations.

<h2><b>Benchmark Your Datasets</b></h2><br>
<b>Select Dataset Type</b>: Choose between Image or Video datasets.
<b>Choose Dataset</b>: Select an available dataset for benchmarking.
<b>Model Selection</b>: Pick the deepfake detection models you want to benchmark your dataset against.
<b>Start Benchmarking</b>: Click the "Benchmark Dataset" button to initiate the benchmarking process.
<br>
The benchmarking results are displayed in detailed bar charts for DeepFake probability and inference time, and a downloadable CSV of the detection results is provided.

## Future Work

FakeSniff aims to incorporate newer models and expand its capabilities to enhance DeepFake detection accuracy and efficiency.

## Contributing

We welcome contributions from the community. Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss the proposed changes.

<h2><b>Acknowledgments</b></h2>

<h3><b>Research & Open-Source Contributions</b></h3>

<table>
  <thead>
    <tr>
      <th>Methods</th>
      <th>Repositories</th>
      <th>Release Date</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>MesoNet</td>
      <td><a href="https://github.com/DariusAf/MesoNet">https://github.com/DariusAf/MesoNet</a></td>
      <td>2018.09</td>
    </tr>
    <tr>
      <td>FWA</td>
      <td><a href="https://github.com/danmohaha/CVPRW2019_Face_Artifacts">https://github.com/danmohaha/CVPRW2019_Face_Artifacts</a></td>
      <td>2018.11</td>
    </tr>
    <tr>
      <td>VA</td>
      <td><a href="https://github.com/FalkoMatern/Exploiting-Visual-Artifacts">https://github.com/FalkoMatern/Exploiting-Visual-Artifacts</a></td>
      <td>2019.01</td>
    </tr>
    <tr>
      <td>Xception</td>
      <td><a href="https://github.com/ondyari/FaceForensics">https://github.com/ondyari/FaceForensics</a></td>
      <td>2019.01</td>
    </tr>
    <tr>
      <td>ClassNSeg</td>
      <td><a href="https://github.com/nii-yamagishilab/ClassNSeg">https://github.com/nii-yamagishilab/ClassNSeg</a></td>
      <td>2019.06</td>
    </tr>
    <tr>
      <td>Capsule</td>
      <td><a href="https://github.com/nii-yamagishilab/Capsule-Forensics-v2">https://github.com/nii-yamagishilab/Capsule-Forensics-v2</a></td>
      <td>2019.1</td>
    </tr>
    <tr>
      <td>CNNDetection</td>
      <td><a href="https://github.com/peterwang512/CNNDetection">https://github.com/peterwang512/CNNDetection</a></td>
      <td>2019.12</td>
    </tr>
    <tr>
      <td>DSP-FWA</td>
      <td><a href="https://github.com/danmohaha/DSP-FWA">https://github.com/danmohaha/DSP-FWA</a></td>
      <td>2019.11</td>
    </tr>
    <tr>
      <td>Upconv</td>
      <td><a href="https://github.com/cc-hpc-itwm/UpConv">https://github.com/cc-hpc-itwm/UpConv</a></td>
      <td>2020.03</td>
    </tr>
    <tr>
      <td>WM</td>
      <td><a href="https://github.com/cuihaoleo/kaggle-dfdc">https://github.com/cuihaoleo/kaggle-dfdc</a></td>
      <td>2020.07</td>
    </tr>
    <tr>
      <td>Selim</td>
      <td><a href="https://github.com/selimsef/dfdc_deepfake_challenge">https://github.com/selimsef/dfdc_deepfake_challenge</a></td>
      <td>2020.07</td>
    </tr>
    <tr>
      <td>Photoshop FAL</td>
      <td><a href="https://peterwang512.github.io/FALdetector/">https://peterwang512.github.io/FALdetector/</a></td>
      <td>2019</td>
    </tr>
    <tr>
      <td>FaceForensics</td>
      <td><a href="https://github.com/ondyari/FaceForensics">https://github.com/ondyari/FaceForensics</a></td>
      <td>2018.03</td>
    </tr>
    <tr>
      <td>CViT</td>
      <td><a href="https://github.com/erprogs/CViT">https://github.com/erprogs/CViT</a></td>
      <td>2021</td>
    </tr>
    <tr>
      <td>Boken</td>
      <td><a href="https://github.com/beibuwandeluori/DeeperForensicsChallengeSolution">https://github.com/beibuwandeluori/DeeperForensicsChallengeSolution</a></td>
      <td>2020</td>
    </tr>
    <tr>
      <td>GANImageDetection</td>
      <td><a href="GANImageDetection">GANImageDetection</a></td>
      <td><a href="License">License</a></td>
    </tr>
  </tbody>
</table>


<h2><b>Developed by:</b></h2>
- Ashutosh Kumar Singh<br>
- Sonu Patel<br>
- Akshay Jain<br>
- Gourav Aggraval<br>

## License

This project is licensed under the MIT License.

## Contact Information

For inquiries or collaborations, please contact us through the GitHub repository.
