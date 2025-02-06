

# 🎥 YouTube Channel Analysis

This project performs **YouTube Channel Analysis** using the **YouTube Data API v3**. It fetches real-time channel statistics such as **subscriber count, total views, and video count**, and generates insights through **data visualization** and **natural language processing (NLP)**.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![YouTube Data API](https://img.shields.io/badge/YouTube-Data%20API-red.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-blue.svg)
![NLP](https://img.shields.io/badge/NLP-WordCloud-yellow.svg)

---

## 📑 Features
- **Real-Time Channel Stats**: Extracts data such as subscriber count, views, total videos, and playlist IDs.
- **Data Visualization**: Generates bar charts and word clouds to visualize key insights.
- **NLP Integration**: Creates word clouds for video metadata analysis.
- **Multi-Channel Support**: Compare multiple YouTube channels at once.

---

## 📂 Project Structure


---

## 🚀 How to Run the Project
1. Clone the repository:
   ```sh
   git clone https://github.com/ASVAHINI/youtube-analysis.git
Install the required dependencies:
sh
Copy
Edit
pip install -r requirements.txt
Open the Jupyter Notebook:
sh
Copy
Edit
jupyter notebook "Youtube analysis.ipynb"
Run each cell to execute the analysis.
🧰 Requirements
Python 3.8 or higher
pandas, matplotlib, seaborn
wordcloud, nltk
google-api-python-client
Install the required packages using:

sh
Copy
Edit
pip install pandas matplotlib seaborn wordcloud nltk google-api-python-client
📊 Sample Code
python
Copy
Edit
# Import required libraries
from googleapiclient.discovery import build
import pandas as pd
from wordcloud import WordCloud
import matplotlib.pyplot as plt

# YouTube Data API initialization
api_key = 'YOUR_API_KEY'
youtube = build('youtube', 'v3', developerKey=api_key)

# Fetch channel statistics
channel_ids = ['UC5EQWvy59VeHPJz8mDALPxg']
request = youtube.channels().list(part="snippet,contentDetails,statistics", id=",".join(channel_ids))
response = request.execute()
🛡️ License
This project is licensed under the MIT License. See the LICENSE file for more details.

💡 Future Improvements
Implement real-time video analysis.
Add sentiment analysis for video comments.
Deploy as a web-based dashboard.



Dashboard
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
An interactive dashboard using Excel is developed for visualizing and exploring the YouTube dataset. Content creators can navigate through various metrics, charts, and visualizations.

![image](https://github.com/user-attachments/assets/eeae42c3-7f4d-42c0-846b-d804d379e8b0)


 Sample Output
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
![image](https://github.com/user-attachments/assets/8b78b6b5-4530-422b-ba12-52d2c09bf053)


![image](https://github.com/user-attachments/assets/efcc1114-dc5a-4164-8956-a220e595981b)


![image](https://github.com/user-attachments/assets/705ef0f0-fc10-4d48-999c-efce020786a6)


![image](https://github.com/user-attachments/assets/cbeac563-aedd-4c6a-913e-25cecda8bf92)


![image](https://github.com/user-attachments/assets/53aabfa5-57a6-46b7-9da2-6a9b5ebdf5ed)


XVI. Conclusion
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
YouTube data analysis offers valuable insights and practical strategies for content creators to improve their channels. By understanding viewer behavior and optimizing strategies, creators can build a loyal audience, increase reach, and achieve long-term success on the platform.
