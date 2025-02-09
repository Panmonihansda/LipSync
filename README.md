# Wav2Lip with GFPGAN Enhancement 🚀

This fork improves video quality using **GFPGAN**, enhancing facial details in generated lip-synced videos.

## 🔹 Improvements
- Integrated **GFPGAN** for better face enhancement.
- Fixed CUDA compatibility & optimized processing.
- Added better error handling.
- **Updated Default Parameters:**
  - `rescaleFactor = 3` (Enhances resolution scaling)
  - `use_hd_model = True` (Uses high-definition GAN model for better lip-sync accuracy)

## HOW TO RUN:
#### git clone https://github.com/Panmonihansda/Wav2Lip.git
#### cd Wav2Lip

### Download Pretrained Models:
#### mkdir -p checkpoints
#### wget -P checkpoints https://www.iiitvadodara.ac.in/pretrained_models/wav2lip_gan.pth

### Run Video Lip-Sync & Enhancement:
#### python inference.py --checkpoint_path checkpoints/wav2lip_gan.pth \
#### --face sample_data/input_vid.mp4 --audio sample_data/input_audio.wav \
#### --pads 0 10 0 0 --resize_factor 3 --nosmooth

Changes in this fork:
--resize_factor 3 → Increases resolution scaling for better clarity.
--checkpoint_path checkpoints/wav2lip_gan.pth → Uses HD model for better accuracy

### Enhance the Output Video using GFPGAN (Optional but Recommended):
#### python enhance_video.py --input results/result_voice.mp4 --output results/result_voice_enhanced.mp4

### Preview the Final Video:
#### from IPython.display import Video
#### Video("results/result_voice_enhanced.mp4")

## 📌 Requirements
```bash
pip install torch torchvision torchaudio
pip install opencv-python numpy scipy librosa soundfile
pip install git+https://github.com/TencentARC/GFPGAN.git













