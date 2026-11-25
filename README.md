# COU07506-labs

Laboratory work for **COU07506** at the Dar es Salaam Institute of Technology (DIT).

| | |
|---|---|
| **Name** | Eliyah Abraham Msangi |
| **Registration No.** | 240141481307 |
| **Programme** | BENG24COE – Bachelor of Engineering in Computer Engineering |

## Week 1 – Discrete-time signals and audio in Python

This repository holds the Week 1 notebook, which covers:

- **Task 1.1** – Elementary sequences: unit impulse δ(n), unit step u(n), unit ramp r(n) and real exponential (0.8)ⁿu(n), drawn as stem plots.
- **Task 1.2** – (1) (a)ⁿu(n) for a = 0.5, −0.8 and 1.1; (2) cos(2πn/8) and cos(2πn/7.5) for 0 ≤ n ≤ 40, and which one repeats exactly.
- **Task 1.3** – Loading a WAV recording, converting stereo to mono, normalising to [−1, 1], and printing the sampling rate, duration and number of samples.
- **Task 1.5** – This Git repository.
- **Analysis questions** – sampling rate and storage per minute, why stem plots are used, and BIBO stability for a = 1.1.

## Files

| File | Description |
|---|---|
| `COU07506_Week01_240141481307.ipynb` | Week 1 notebook (code, plots, answers) |
| `my_voice.wav` | Voice recording used in Task 1.3: "GLORY TO ALMIGHTY GOD OF HEAVEN" |
| `requirements.txt` | Python packages used |
| `README.md` | This file |

## How to run (Google Colab)

1. Open <https://colab.research.google.com> and choose **File → Upload notebook**. Select `COU07506_Week01_240141481307.ipynb`.
2. Open the **Files** panel (folder icon on the left) and upload `my_voice.wav`.
3. Choose **Runtime → Run all**.

The notebook prints the sampling rate `fs`, the duration and the number of samples of `my_voice.wav`. If the file is not found, it uses a fallback test signal (a decaying 440 Hz tone, 2 s at 16 kHz).

## How `my_voice.wav` was recorded (Audacity)

1. Install Audacity (<https://www.audacityteam.org>), connect a microphone and press **Record**.
2. Say clearly: **"GLORY TO ALMIGHTY GOD OF HEAVEN"** (3–5 seconds), then press **Stop**.
3. Choose **File → Export → Export as WAV**, save as `my_voice.wav` with the encoding **Signed 16-bit PCM**.

A phone recording can be converted to WAV in Audacity with the same export step.

## Requirements

Python 3, NumPy, SciPy and Matplotlib (all pre-installed in Google Colab). To run locally: `pip install -r requirements.txt`.
