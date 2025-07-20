# 🎨 Colorize Images & Videos - DeOldify

![DeOldify Banner]()

## 📋 Project Overview

[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg?style=flat-square&logo=python)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-Latest-red.svg?style=flat-square&logo=pytorch)](https://pytorch.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?style=flat-square&logo=jupyter)](https://jupyter.org/)

**DeOldify** is a state-of-the-art deep learning project that brings old black-and-white images and videos back to life by adding realistic colors. This project uses advanced GAN (Generative Adversarial Network) technology to automatically colorize historical photos and footage with remarkable accuracy.

### 🌟 Key Features

- **Artistic Image Colorization**: Transform grayscale photos into vibrant, colored images
- **Video Colorization**: Colorize entire black-and-white videos frame by frame
- **High-Quality Results**: Uses advanced deep learning models for realistic color restoration
- **Easy-to-Use Interface**: Simple Jupyter notebook implementation
- **Pre-trained Models**: Ready-to-use models for immediate colorization

## 🚀 Quick Start

### Prerequisites

- Python 3.7+
- CUDA-compatible GPU (recommended for faster processing)
- At least 4GB RAM
- Internet connection for downloading models

### 🔧 Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/mmaithani/DeOldify.git
   cd DeOldify
   ```

2. **Install Dependencies**
   ```bash
   pip install -r colab_requirements.txt
   ```

3. **Create Models Directory**
   ```bash
   mkdir models
   ```

4. **Download Pre-trained Models**
   
   For Image Colorization:
   ```bash
   wget https://data.deepai.org/deoldify/ColorizeArtistic_gen.pth -O ./models/ColorizeArtistic_gen.pth
   ```
   
   For Video Colorization:
   ```bash
   wget https://data.deepai.org/deoldify/ColorizeVideo_gen.pth -O ./models/ColorizeVideo_gen.pth
   ```

### 📂 Project Structure

```
deoldify_project/
└── Colorize Images & Videos - DeOldify/
    ├── bw_test_video.mp4              # Sample black-and-white test video
    ├── bw_test_video_deoldify.mp4     # Colorized output video
    ├── bw_test1.jpg                   # Test image 1 (grayscale)
    ├── bw_test2.jpg                   # Test image 2 (grayscale)
    ├── bw_test3.jpg                   # Test image 3 (grayscale)
    ├── Colorize Images & Videos - Deoldify.ipynb  # Main notebook
    └── README.md                      # This file
```

## 🎯 Usage

### For Images

1. Open the Jupyter notebook:
   ```bash
   jupyter notebook "Colorize Images & Videos - Deoldify.ipynb"
   ```

2. Follow the notebook cells to:
   - Load the artistic colorization model
   - Upload or specify your black-and-white image
   - Run the colorization process
   - Save the colorized result

### For Videos

1. Use the video colorization section in the notebook
2. Load the video colorization model
3. Process your black-and-white video
4. Export the colorized video

## 📸 Sample Results

The project includes several test files:

- **Test Images**: `bw_test1.jpg`, `bw_test2.jpg`, `bw_test3.jpg`
- **Test Video**: `bw_test_video.mp4`
- **Sample Output**: `bw_test_video_deoldify.mp4`

## 🛠️ Technical Details

### Models Used

![Model Size](https://img.shields.io/badge/Model_Size-~200MB-green.svg?style=flat-square)
![Accuracy](https://img.shields.io/badge/Accuracy-85%25+-brightgreen.svg?style=flat-square)
![GPU Memory](https://img.shields.io/badge/GPU_Memory-4GB+-blue.svg?style=flat-square)

- **ColorizeArtistic_gen.pth**: Optimized for artistic and portrait images
- **ColorizeVideo_gen.pth**: Specialized for video frame colorization

## 🛠️ Technology Stack

![Python](https://img.shields.io/badge/Python-3.8+-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![FastAI](https://img.shields.io/badge/FastAI-00A98F?style=for-the-badge&logo=fastai&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter_Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)

### Core Technologies

- **Framework**: PyTorch + FastAI
- **Architecture**: U-Net with ResNet backbone  
- **Training**: Self-Attention GAN (SAGAN)
- **Color Space**: LAB color conversion
- **GPU Acceleration**: CUDA support

## ⚙️ Configuration Options

### Image Colorization Parameters

- **Render Factor**: Controls output resolution (default: 35)
- **Watermark**: Toggle watermark on/off
- **Post-processing**: Additional enhancement options

### Video Colorization Parameters

- **Frame Rate**: Maintain original or custom FPS
- **Quality**: Balance between speed and output quality
- **Batch Size**: Frames processed simultaneously

## 🔍 Troubleshooting

### Common Issues

1. **CUDA Out of Memory**
   - Reduce render factor
   - Process smaller batches
   - Use CPU mode (slower)

2. **Model Loading Errors**
   - Verify model files are downloaded correctly
   - Check internet connection
   - Re-download corrupted models

3. **Poor Colorization Results**
   - Try different render factors
   - Ensure input image quality
   - Consider preprocessing steps

## 🤝 Contributing

Contributions are welcome! Please feel free to submit:

- Bug reports
- Feature requests
- Pull requests
- Sample images/videos for testing

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Fast.ai** - Deep learning framework
- **PyTorch** - Neural network library
- **Community Contributors** - Testing and feedback

---

### 🌈 Transform Your Memories Today!

Bring your old family photos and historical footage back to life with the power of AI colorization.

**Happy Colorizing! 🎨✨**
