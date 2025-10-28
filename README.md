# 🎨 R3ND3R-9

A powerful Streamlit app for generating professional product ads using Bria AI's advanced image generation and manipulation APIs. The next generation of visual creation tools.

## 🌟 Features

- 🖼️ Generate HD product images from text prompts
- 🎯 Remove backgrounds with custom colors
- 🌅 Add realistic shadows
- 🏠 Create lifestyle shots with text or reference images
- ✨ AI-powered prompt enhancement
- 📝 Optional CTA text overlay
- 🎮 Intuitive UI controls
- 💾 Easy image download

## 🚀 Quick Start

1. Clone the repository:
```bash
git clone https://github.com/Adams-404/R3ND3R-9.git
cd R3ND3R-9
```

2. Create and use a virtual environment (recommended):
```bash
# Create a venv (Python 3.10 recommended)
python3.10 -m venv .venv

# Activate it (Linux/macOS)
source .venv/bin/activate

# Install dependencies inside the venv
pip install -r requirements.txt
```

3. Create a `.env` file in the root directory:
```bash
BRIA_API_KEY=your_api_key_here
```

4. Run the app:
```bash
# If the venv is activated
streamlit run app.py

# Or without activating the venv
.venv/bin/streamlit run app.py
```

## 💡 Usage

1. Enter a product description or upload an image
2. Configure generation options in the sidebar:
   - Enhance prompt with AI
   - Remove background
   - Add shadows
   - Generate lifestyle shots
3. Adjust advanced settings like background color and shadow intensity
4. Click "Generate Ad" to create your images
5. Download the results

## 🔧 Configuration

The app supports various configuration options through the UI:

- **Prompt Enhancement**: Improve your text prompts with AI
- **Background Removal**: Remove backgrounds with custom colors
- **Shadow Effects**: Add realistic shadows with adjustable intensity
- **Lifestyle Shots**: Place products in context using text or reference images
- **CTA Text**: Add optional call-to-action text overlays

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## 🧰 Troubleshooting

- Pillow build error on Python 3.13
  - Symptom: Installing `Pillow==10.2.0` fails with a build or `KeyError: '__version__'` when using Python 3.13.
  - Fix: Use the provided project virtual environment with Python 3.10, or upgrade Pillow to a Python 3.13 compatible version. This project pins `Pillow==10.2.0`, which has prebuilt wheels for Python 3.10.

- Missing module `streamlit_drawable_canvas`
  - Ensure dependencies are installed inside the venv: `pip install -r requirements.txt` after activating the venv, or run with `.venv/bin/streamlit run app.py`.
  - We've pinned `streamlit-drawable-canvas==0.9.3` in `requirements.txt`.

- Environment variables not loading
  - Verify `.env` exists at the project root and contains `BRIA_API_KEY=...`.
  - The app loads environment variables using `python-dotenv` at startup.
