 ***Traffic Flow Prediction using NLP***
 ---
 
This project aims to provide a real-time traffic prediction system that uses geolocation (latitude and longitude) and user-described traffic situations to forecast traffic flow. By integrating machine learning and natural language processing (NLP). This helps users plan safer and more efficient routes across different locations.

## Directions to use this repo:

- Clone the repository by running:  
  `git clone https://github.com/JyothsnaDarla/traffic-prediction.git`
- Install all dependencies:  
  `pip install -r requirements.txt`
- Run the application:  
  `python app.py`
- Visit the app in your browser:  
  `http://127.0.0.1:5000/`

  ## Dataset
  This project uses a custom dataset prepared manually for traffic flow prediction using Natural Language Processing (NLP) techniques combined with geographical data. Unlike generic or publicly available datasets, this one has been carefully crafted to reflect real-world urban traffic conditions and language patterns. Each record contains a location name, its corresponding latitude and longitude, a textual description of the traffic situation, and a label indicating the severity of traffic flow. The label is marked as 0 for low or smooth traffic and 1 for heavy or congested traffic.

***How It Works***
---

The user enters a city name, optionally a street name, and a traffic-related description (e.g., "construction", "evening rush", "accident near market").
The system extracts the latitude and longitude using the Geopy library.
Two machine learning models are used:
A text-based model using TF-IDF and Random Forest
A location-based model using latitude and longitude
The final prediction combines both model results (and historical data if available) to classify traffic as:
Smooth Traffic,Moderate Traffic,Heavy Traffic
Results are displayed on an interactive map, and also stored in an SQLite database.

 ***Key Features***
 ---
Real-time traffic prediction using both location and description
NLP preprocessing using NLTK
Geolocation with Nominatim (Geopy)
Map visualization using Folium
Historical data tracking via SQLite
Easy-to-use web interface built with Flask

**Home page:**
Introduction to the application
![Image](https://github.com/user-attachments/assets/1015e9e0-5fd5-4007-ac21-b059c667f83b)
**Entry page:**
Form to input traffic details and get prediction
![Image](https://github.com/user-attachments/assets/423d346f-87f1-4bdc-a73b-4550aef8f531)
**result page:**
Shows traffic prediction and map
![Image](https://github.com/user-attachments/assets/ac152ec3-a3c7-4216-b31f-0c058d8421ad)
**show page:**
Displays recent predictions for selected location
![Image](https://github.com/user-attachments/assets/d2c283e5-b2c3-4aba-9510-82d9d380d63a)

**Objective:**
---
This project aims to reduce traffic-related stress by helping users avoid congested routes. It supports smarter commuting decisions and promotes better traffic flow management using a data-driven approach.
