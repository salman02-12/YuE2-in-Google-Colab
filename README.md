# ⚡ YuE2 Music Generation in Google Colab

This repository provides an easy-to-use Google Colab notebook to run **YuE2**, an advanced AI music generation model. Built on ComfyUI, this tool allows you to create complete songs with vocals from scratch (Text-to-Music) or generate customized covers of existing songs (Music Cover), all running locally on a free Google Colab T4 GPU.

**🎥 Watch the Tutorial:** [How to Use](https://www.youtube.com/watch?v=soon)

**🚀 Run in Colab:** [Open Google Colab Notebook](https://colab.research.google.com/drive/15xKI5kv6BpiB4aTx7zjzgI0rZugY2qpM?usp=sharing)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salman02-12/YuE2-in-Google-Colab/blob/main/YuE2_CoinNoin.ipynb)
[![Get Pro](https://img.shields.io/badge/Get%20Pro-PayPal-blue?logo=paypal)](https://www.paypal.com/ncp/payment/9592PQ88FJDJC)

---
<img src="./thumbnail.png" width="100%" />

## ✨ Features Supported in this Notebook

This notebook streamlines the complex YuE2 music generation process into simple steps:

1. **⚙️ Initialize Core Environment**: Automatically sets up the ComfyUI engine and essential dependencies for native YuE2 nodes.
2. **📥 Download YuE2 Models**: Rapidly fetches the 3B parameter YuE2 checkpoint. It also includes an optional download for the **SheetSage2 audio encoder**, which is required if you want to create song covers.
3. **🎵 YuE2 Text to Music**: 
   * Generate a complete song (vocals and instruments) simply by providing a text description of the style (e.g., "contemporary pop, 96 BPM") and writing your own lyrics.
   * Supports **ABC Planning**: The AI can write an editable melody/chord plan before rendering the audio for better musical structure.
   * Control the max duration (up to 900 seconds) and generation mode (full song or melody only).
4. **🎤 YuE2 Music Cover**: 
   * Upload an existing `.flac`, `.wav`, or `.mp3` song.
   * The SheetSage2 encoder transcribes the original melody, and YuE2 re-sings it using your newly provided lyrics and musical style!

## 🛠️ How to Use

1. Click the "Open in Colab" badge above.
2. Go to **Runtime > Change runtime type** and ensure the **T4 GPU** is selected in Colab.
3. Run **Cell 1** to initialize the ComfyUI environment.
4. Run **Cell 2** to download the models. Make sure `DOWNLOAD_SHEETSAGE2` is checked if you want to make covers.
5. **To generate a new song:** Go to **Cell 3**, type your music style and lyrics (using tags like `[Verse]`), and click Play.
6. **To make a cover:** Go to **Cell 4**, type your new style and lyrics, and click Play. You will be prompted to upload your reference song.
7. *Note: YuE2 is a large model. Song generation will take several minutes on a T4 GPU.*

## 🤝 Credits
* **Notebook Creator:** [@CoinNoin](https://www.youtube.com/@CoinNoin)
* **Base Models:** [Comfy-Org / YuE2](https://huggingface.co/Comfy-Org/YuE2)
