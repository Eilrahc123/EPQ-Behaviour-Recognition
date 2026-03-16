# EPQ-Behaviour-Recognition

## Project Introduction
This project implements a real-time student behaviour detection system using **LSTM** (Long Short-Term Memory) and **Mediapipe**. 

## Technical Evolution
To achieve high inference speed on a desktop environment, the project pipeline follows:
1. **Framework Selection**: Adapted an action recognition framework, refactoring it for classroom behaviour scenarios.
2. **Data Pipeline**: Customized `data_collection.ipynb` to capture 30 frames of keypoints per action.
3. **Model Optimization**: The model was converted from `.h5` to `.onnx` for 2x faster performance.

## File Guide
- `task4_realtime.ipynb`: **Core logic** (The primary application).
- `LSTM_train.ipynb`: Training script with custom categorical cross-entropy.
- `Convert_to_ONNX.ipynb`: Optimization script for deployment.

*Note: Some legacy scripts contain references to the base framework's original sign-language annotations, which were utilized for structural reference during initial development.*