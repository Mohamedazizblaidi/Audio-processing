# 🎵 Audio Processing

A Python-based audio analysis and visualization project using **Librosa**, designed to explore and process audio files (`.wav`) through spectral analysis, waveform visualization, and feature extraction.

---

## 📁 Project Structure

```
Audio-processing/
│
├── Audio processing.ipynb   # Main Jupyter notebook
├── *.wav                    # Audio files used for analysis
└── README.md
```

---

## 🔧 Requirements

Make sure you have **Python 3.x** installed, then install the dependencies:

```bash
pip install librosa numpy pandas matplotlib seaborn IPython
```

Or using a `requirements.txt`:

```bash
pip install -r requirements.txt
```

### Dependencies

| Library | Purpose |
|---|---|
| `librosa` | Audio loading, feature extraction, display |
| `numpy` | Numerical operations |
| `pandas` | Data handling |
| `matplotlib` | Plotting and visualization |
| `seaborn` | Plot styling |
| `IPython` | Audio playback in Jupyter |

---

## 🚀 Getting Started

1. **Clone the repository**

```bash
git clone https://github.com/your-username/Audio-processing.git
cd Audio-processing
```

2. **Install dependencies**

```bash
pip install librosa numpy pandas matplotlib seaborn IPython
```

3. **Launch the notebook**

```bash
jupyter notebook "Audio processing.ipynb"
```

4. Place your `.wav` audio files in the project directory and update the file paths in the notebook accordingly.

---

## 📊 Features

- **Waveform visualization** — plot raw audio signal over time
- **Spectrogram analysis** — visualize frequency content using Short-Time Fourier Transform (STFT)
- **Mel spectrogram** — perceptually-scaled frequency representation
- **Audio playback** — listen to audio directly inside the Jupyter notebook via `IPython.display`
- **Batch processing** — load and process multiple `.wav` files using `glob`
- **Color-cycled plots** — styled visualizations using Seaborn and Matplotlib color palettes

---

## 📌 Usage Example

```python
import librosa
import librosa.display
import matplotlib.pyplot as plt

# Load audio file
y, sr = librosa.load("your_audio.wav")

# Plot waveform
plt.figure(figsize=(14, 5))
librosa.display.waveshow(y, sr=sr)
plt.title("Waveform")
plt.show()
```

---

## 📄 License

This project is open-source. Feel free to use and modify it for your own audio analysis needs.
