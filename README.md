# DeepFakes-Detection

```markdown
## My Approach -
### How It Works 💡
- We take 15 uniformly time-spaced frames from the video and work upon them.
- Then we crop out the area around the person's face in each frame using the Harrcascade module.
- Harrcascade performs pixel-wise face localisation on various scales of faces by taking advantages of joint extra-supervised and self-supervised multi-task learning. 
- We use Harrcascade with Resnet-50 as the encoder model.
- After getting the cropped face we normalizing it and resize every pictures to (320,320,3) shape, i.e. an rgb image of 320px * 320px
- We finally use an ensemble of Efficient-Net and Xception net by getting there predictions as probabilites and then try out different ratios for the both of them.
- The best ratio was with giving 30% weightage to the xception model's score and 70% to the efficient net model.

## Results
- This model acheived 2nd place in the [DeepFake Detection Challenge hosted on Kaggle](https://www.kaggle.com/competitions/deepfake-detection/overview)
- F1 Score on the testing dataset = 0.861



# Deepfake Videos Detection 🔍🎥




## Results 📊
- **Precision**: 0.88
- **Recall**: 0.85
- **F1 Score**: 0.861

The combination of computer vision techniques and cutting-edge deep learning models makes this system highly efficient in identifying Deepfakes in videos.

## Project Timeline
**December 2023**

---

## Contributions
Feel free to contribute by submitting pull requests or opening issues. We welcome any ideas to improve the accuracy, speed, or feature set of this project.


```

This README is designed to be both informative and engaging, using a combination of emojis and well-structured sections to keep it eye-catching while providing a clear overview of the project.
