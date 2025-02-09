# LipSync


# Wav2Lip with GFPGAN Enhancement 🚀

This fork improves video quality using **GFPGAN**, enhancing facial details in generated lip-synced videos.

## 🔹 Improvements
- Integrated **GFPGAN** for better face enhancement.
- Fixed CUDA compatibility & optimized processing.
- Added better error handling.

## 📌 Requirements
```bash
pip install torch torchvision torchaudio
pip install opencv-python numpy scipy librosa soundfile
pip install git+https://github.com/TencentARC/GFPGAN.git
