
#  ASL Alphabet Interpreter  
Recognize American Sign Language letters using deep learning!

This project trains a Convolutional Neural Network (CNN) to classify hand gestures from grayscale images into 29 classes — the English alphabet (A–Z), plus `space` and `nothing`. It supports training, webcam inference, and browser deployment via TensorFlow.js.

---

## 🚀 Features

-  29-class classification: A–Z, space, nothing  
-  Trained on 87,000+ preprocessed hand gesture images  
-  Run predictions in real time using your webcam  
-  Exportable to TensorFlow.js for browser-based use  
-  Fully modular: dataset → training → model → deployment



## Project Structure



asl-interpreter/
├── model/                      
│   ├── asl\_cnn\_model.keras
│   ├── asl\_label\_encoder.pkl
│   └── convert\_to\_tfjs.sh
│
├── dataset/                    
│   ├── asl\_alphabet\_full.csv
│   └── sample\_images/
│
├── notebooks/                 
│   └── train\_model.ipynb
│
├── scripts/                    
│   ├── train\_model.py
│   └── live\_predict.py
│
├── tfjs\_model/                 
│   ├── model.json
│   └── group1-shard1of1.bin
│
├── webapp/                     
│   ├── index.html
│   ├── app.js
│   └── style.css
│

└── README.md




Required packages:

tensorflow
pandas
numpy
scikit-learn
opencv-python
matplotlib
joblib



##  Dataset

The dataset was sourced from [Kaggle: ASL Alphabet Dataset](https://www.kaggle.com/datasets/grassknoted/asl-alphabet) and converted into a single `.csv` with pixel-normalized grayscale values for training.

### Label Map:


A → 0, B → 1, ..., Z → 25, space → 26, nothing → 27





##  Acknowledgments

* Dataset by [grassknoted on Kaggle](https://www.kaggle.com/datasets/grassknoted/asl-alphabet)
* Help of A.I. tools for brainstorming





