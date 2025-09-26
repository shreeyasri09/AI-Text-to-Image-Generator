# AI Text to Image Generator

A powerful AI-powered text-to-image generator using Stable Diffusion v1.5. This project allows you to create stunning images from text descriptions with intelligent prompt optimization and token management.

## 🚀 Features

- **Smart Prompt Optimization**: Automatically detects and optimizes prompts that exceed the 77-token limit
- **Token Management**: Real-time token counting and warnings
- **Device Detection**: Automatically detects and uses available hardware (GPU/CPU)
- **Error Handling**: Comprehensive error handling with helpful suggestions
- **Interactive Interface**: User-friendly prompts and progress indicators

## 📋 Requirements

- Python 3.8+
- CUDA-compatible GPU (recommended) or CPU
- Hugging Face account and access token

## 🛠️ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ai-text-to-image-generator.git
   cd ai-text-to-image-generator
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up Hugging Face token:**
   - Get your token from [Hugging Face Settings](https://huggingface.co/settings/tokens)
   - **Option A**: Set environment variable: `set HF_TOKEN=your_token_here` (Windows) or `export HF_TOKEN=your_token_here` (Mac/Linux)
   - **Option B**: Enter token when prompted in the notebook
   - **Option C**: Use command line: `python text_to_image_generator.py --token your_token_here`

## 🎯 Usage

### Option 1: Jupyter Notebook
1. Open `AI_Text_to_Image_Generator.ipynb`
2. Run all cells in order
3. Enter your text prompt when prompted
4. Wait for the image generation to complete

### Option 2: Google Colab (Recommended)
1. Upload the notebook to Google Colab
2. Change runtime to GPU (Runtime → Change runtime type → GPU)
3. Run all cells
4. Enjoy fast image generation!

## 📝 Example Prompts

**Good prompts (under 77 tokens):**
- "A serene mountain landscape at sunset with a lake reflection"
- "A futuristic city with flying cars and neon lights"
- "A cozy cabin in a snowy forest with warm lights"

**The system will automatically optimize longer prompts like:**
- "A young woman named Mekhala sitting peacefully on a wooden bench in a vibrant, sunlit garden in the USA, enjoying an ice cream cone..."

## ⚙️ Configuration

### Model Settings
- **Model**: `runwayml/stable-diffusion-v1-5`
- **Image Size**: 512x512 pixels
- **Inference Steps**: 50 (adjustable)
- **Guidance Scale**: 7.5 (how closely to follow the prompt)

### Hardware Requirements
- **GPU**: NVIDIA GPU with CUDA support (recommended)
- **CPU**: Works but very slow (10-20 minutes per image)
- **RAM**: 8GB+ recommended

## 🔧 Troubleshooting

### Common Issues

1. **Token Length Exceeded**
   - The system will automatically suggest optimized prompts
   - Keep prompts under 77 tokens for best results

2. **CUDA Not Available**
   - Use Google Colab with GPU for better performance
   - CPU mode will work but be very slow

3. **Memory Issues**
   - Reduce image size or inference steps
   - Use a machine with more RAM

4. **Authentication Errors**
   - Ensure your Hugging Face token is valid
   - Check token permissions

## 📊 Performance

| Hardware | Generation Time | Quality |
|----------|----------------|---------|
| T4 GPU (Colab) | 30-60 seconds | High |
| A100 GPU | 15-30 seconds | High |
| CPU | 10-20 minutes | High |

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [Hugging Face](https://huggingface.co/) for the Stable Diffusion model
- [RunwayML](https://runwayml.com/) for the base model
- [Diffusers](https://github.com/huggingface/diffusers) library

## 📞 Support

If you encounter any issues or have questions, please open an issue on GitHub.

---

**Happy Image Generating! 🎨✨**
