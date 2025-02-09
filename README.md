# Wav2Lip with GFPGAN Enhancement 🚀

This fork improves video quality using **GFPGAN**, enhancing facial details in generated lip-synced videos.

## 🔹 Improvements
- Integrated **GFPGAN** for better face enhancement.
- Fixed CUDA compatibility & optimized processing.
- Added better error handling.
- **Updated Default Parameters:**
  - `rescaleFactor = 3` (Enhances resolution scaling)
  - `use_hd_model = True` (Uses high-definition GAN model for better lip-sync accuracy)

## 📌 Requirements
```bash
pip install torch torchvision torchaudio
pip install opencv-python numpy scipy librosa soundfile
pip install git+https://github.com/TencentARC/GFPGAN.git



