---

# Deepfake Detection System 🔍🎥

Deepfakes have emerged as a serious challenge in the digital age, blurring the lines between reality and manipulation. Our system leverages advanced computer vision techniques and state-of-the-art deep learning models to detect deepfake videos with high accuracy. This project was ranked **2nd place** in the [Kaggle DeepFake Detection Challenge](https://www.kaggle.com/competitions/deepfake-detection/overview), achieving an impressive **F1 score of 0.861**!

---

## How It Works 💡

1. **Frame Selection**: We extract 15 uniformly spaced frames from the video, ensuring we capture the subject’s facial movements throughout.
   
2. **Face Detection**: Using the Haar Cascade Classifier, we localize the face in each frame. This method is a powerful pixel-wise face localization tool that works across multiple face scales by employing a combination of joint extra-supervised and self-supervised multi-task learning.

3. **Deep Learning Backbone**: The face regions are cropped, normalized, and resized to a consistent dimension of **320x320 pixels** (RGB format). 

4. **Model Ensemble**:
   - We harness the power of two robust models: **EfficientNet** and **Xception**. 
   - By fusing their predictions with a weighted ensemble, where EfficientNet contributes **70%** and Xception adds **30%** to the final score, we capture diverse feature representations from the frames.

5. **Prediction**: The ensemble's combined score helps classify whether the video is real or deepfake.

---

## Performance Metrics 📊

- **Precision**: 0.88
- **Recall**: 0.85
- **F1 Score**: 0.861

This balanced combination of precision and recall highlights the robustness of the system in detecting deepfakes, minimizing both false positives and false negatives.

---

## Project Timeline 🗓️

- **December 2023**: Project development and Kaggle submission

---

## How to Contribute 💻

We invite developers and researchers to contribute to this project. Whether you want to improve accuracy, enhance speed, or add new features, your ideas are welcome! Simply submit a **pull request** or open an **issue**. Let’s collaborate to combat the threat of deepfake videos together.

---

## Acknowledgments 🙌

A huge thanks to Kaggle for hosting the challenge and to the entire open-source community for the valuable tools and resources that made this project possible.

--- 

Together, let’s keep our digital world safer from misinformation! 💻✨

