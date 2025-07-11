# 😷 Mask Detection Using CNN

A computer vision project that uses a Convolutional Neural Network (CNN) to detect whether a person is wearing a face mask or not. Built with **Python**, **TensorFlow**, **Keras**, **OpenCV**, and **NumPy**, this project includes data preprocessing, CNN training, and real-time mask detection via webcam.

---

## 📁 Project Structure

```bash
.
├── 1_0_data_preprocessing.ipynb       # Dataset loading and preprocessing
├── 2_0_training_the_CNN.ipynb         # Model building and training
├── 3_0_detecting_Masks.ipynb          # Real-time or image-based mask detection
├── haarcascade_frontalface_default.xml # Face detection using OpenCV
└── README.md
````

---

## 📦 Dataset & Trained Model

📥 Download from Google Drive:
[➡️ Dataset + Trained Model](https://drive.google.com/drive/folders/1rIbJAryC1QPYI_i8DYD9fWMGRzZmmSA1?usp=sharing)

After downloading:

* Place the dataset in a folder (e.g., `dataset/`)
* Place the trained model in a same folder as code (e.g., `/`) as referenced in your notebooks

---

## 🛠️ Getting Started

You can run the project using **Jupyter Notebook** or **Google Colab**.

---

### 💻 Option 1: Run in Jupyter Notebook

1. Open the notebooks in order:

   * `1_0_data_preprocessing.ipynb`
   * `2_0_training_the_CNN.ipynb`
   * `3_0_detecting_Masks.ipynb`

2. Make sure `haarcascade_frontalface_default.xml` is in the same directory as the detection notebook.

---

### ☁️ Option 2: Run in Google Colab (Recommended)

1. Upload the `.ipynb` files to Colab or open them from GitHub.

2. Install required libraries at the top of each notebook:

   ```python
   !pip install numpy opencv-python tensorflow keras
   ```

3. Upload the `haarcascade_frontalface_default.xml` file:

   ```python
   from google.colab import files
   files.upload()
   ```

4. Upload your dataset and trained model manually, or mount Google Drive:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

---

## 🔍 Notebook Workflow

### 1️⃣ `1_0_data_preprocessing.ipynb`

* Loads the image dataset
* Labels images as "mask" or "no mask"
* Prepares data for training

### 2️⃣ `2_0_training_the_CNN.ipynb`

* Builds a CNN using Keras
* Trains and evaluates the model
* Saves the trained model (`.h5`)

### 3️⃣ `3_0_detecting_Masks.ipynb`

* Loads the saved model
* Uses OpenCV and Haar cascades to detect faces
* Predicts mask status (real-time or image)

---

## 🧾 Requirements

Listed in `requirements.txt`:

```
numpy>=1.21.0
opencv-python>=4.5.0
tensorflow>=2.8.0
keras>=2.8.0
```

Install manually if needed:

```bash
pip install numpy opencv-python tensorflow keras
```

---

## 📷 Sample Output

* ✅ Mask detected → Green box around the face
* ❌ No mask detected → Red box around the face

---

## 🙏 Acknowledgements

* TensorFlow & Keras — Deep learning framework
* OpenCV — Real-time face detection
* Dataset provided via the [Google Drive link](https://drive.google.com/drive/folders/1rIbJAryC1QPYI_i8DYD9fWMGRzZmmSA1?usp=sharing)

---

## 📝 License

This project is open-source and intended for educational and research purposes. I would appreciate the contribution.
