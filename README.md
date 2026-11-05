# Indian Sign Language Recognition (CNN-LSTM vs Transformer)

Deep learning system that recognises 8 Indian Sign Language emergency words
(accident, call, doctor, help, hot, lose, pain, thief) from video.

## How it works
- MediaPipe hand landmarks: 126 features per frame (21 points × 3 coords × 2 hands)
- Sequences padded to 45 frames and min–max normalised
- Three models trained and compared: CNN-LSTM, Transformer, Hybrid CNN-Transformer
- Attention visualisation for interpretability
- Live dashboard that predicts from an uploaded video or photo

## Results (test accuracy)
| Model | Accuracy |
|---|---|
| CNN-LSTM | 91.94% |
| Transformer | 90.32% |
| Hybrid CNN-Transformer | 75.81% |

## Files
- `ISL_train.ipynb`: preprocessing, model training and evaluation
- `ISL_demo.ipynb`: prediction demo on new videos and images

## Dataset
"A Video Dataset of Hand Gestures of Indian Sign Language Words used in
Emergency Situations" (Mendeley Data): 412 clips, 26 signers.

## Author
Diya Mary George, MCA, Rajagiri College of Social Sciences
