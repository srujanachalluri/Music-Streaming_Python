# 🎵 Music Streaming Genre Prediction

[![Python](https://img.shields.io/badge/Python-3.x-blue)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange)](https://scikit-learn.org/stable/)
[![Pandas](https://img.shields.io/badge/Pandas-1.x-green)](https://pandas.pydata.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A **Machine Learning** project that predicts a user's preferred music genre based on their **age** and **gender**, using a **Decision Tree Classifier**.

---

## 📌 Problem Statement

- **Males** aged **20–25** → like **HipHop** 🎤  
- **Females** aged **20–25** → like **Dance** 💃  

The model can **generalize to unseen ages**.  
Example: If the dataset does not contain age **21**, the model should still predict accurately.

---

## 🛠 Project Workflow

flowchart TD
    A[📥 Import Data] --> B[🧹 Clean Data]
    B --> C[✂️ Split Data]
    C --> D[🛠 Create Model]
    D --> E[📚 Train Model]
    E --> F[🔮 Make Predictions]
    F --> G[📊 Evaluate & Improve]


---

## Dataset
`music.csv` contains:
| age | gender | genre  |
|-----|--------|--------|
| 20  | 1      | HipHop |
| 23  | 1      | HipHop |
| 25  | 1      | HipHop |
| 26  | 1      | Jazzz  |
| 29  | 1      | Jazzz  |

- **age**: Numeric age of the user.
- **gender**: Encoded (1 = Male, 0 = Female).
- **genre**: Target label (preferred music genre).

---

## Example Prediction
python
predictions = model.predict([[21, 1], [21, 0]])
# Output: ['HipHop', 'Dance'] 

The dataset can be viewed here: [music.csv](https://raw.githubusercontent.com/srujanachalluri/Music-Streaming_Python/main/music.csv)

---

📊 Model Performance
Accuracy: ~50% on test data

- Can be improved by:

- Adding more training data

- Using advanced algorithms (Random Forest, SVM)

- Feature engineering

---

## Requirements
  pip install pandas scikit-learn
  
## How to Run

Clone the repository. (git clone https://github.com/srujanachalluri/Music-Streaming_Python.git)
Add music.csv to the project folder.
Run the Python script. (python music_streaming.py)
Use model.predict() to classify new data points.

Music Streaming
Execution steps:

Clone from Github repo and do the modifications and push back to git:
1.   git clone https://github.com/yourusername/music-streaming.git
2.   cd music-streaming
For any modifications, make the changes and push to Github using below commands: 
1.    git add .
2.    git commit -m "Update music.ipynb and music.csv"
3.    git push origin main
verify in Github

For execution :
Make sure the music.csv file is in the path /content/sample_data/music.csv
Open Google colaboratory and run the file music.ipynb

## Results

You can view the results [here](ResultAccuracySS.png)

## 🚀 Live Demo

### Open in Google Colab
You can launch the notebook directly in Colab (no local install needed):

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/srujanachalluri/Music-Streaming_Python/blob/main/Music_Streaming_Project.ipynb)

---
📜 License
This project is licensed under the MIT License - see the LICENSE file for details.

💡 Author
Developed by Srujana Challuri 🚀
