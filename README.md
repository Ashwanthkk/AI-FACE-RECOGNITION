# 🤖 AI Face Recognition

AI Face Recognition is a deep learning project that uses a **Convolutional Neural Network (CNN)** to detect and recognize human faces from images and video streams. The system supports training on a custom dataset and performing face recognition on both static images and real-time video.

---

## 🛠️ Technologies Used

- 🧠 **PyTorch** – For building and training the neural network  
- 🎥 **OpenCV** – For video capture and image processing  
- 🖼️ **Pillow (PIL)** – For image handling and preprocessing  
- 🕸️ **CNN (Convolutional Neural Network)** – Core model for facial feature extraction and classification  

---

## 📁 Project Structure

- **`training the model.py`**  
  🏋️ Trains the CNN model using labeled images. After training, it generates:
  - ✅ `weights(Familycnn)` file (model parameters)
  - ✅ `idx_to_class` file (label-to-name mapping)

- **`predict the face.py`**  
  🎞️ Recognizes the face owner in a **video stream** using the trained model (webcam or file).

- **`predictimage.py`**  
  🖼️ Recognizes the face owner in a **photo** using the trained model.

---

## ⚠️ Notes

- The `weights(Familycnn)` and `idx_to_class` files are **not provided** in this repo.
- These files are **automatically created** after completing training using `training the model.py`.

---

## ❗ Limitations

- If the training dataset is **too small**, the model may **overfit**, leading to poor generalization on new data.

---

## 📦 Installation

Install the required Python libraries:

```bash
pip install torch torchvision opencv-python Pillow
