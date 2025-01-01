# **Real Estate AI Assistant**

### **Overview**
The Real Estate AI Assistant is a Python-based tool designed to simplify the property search process. It integrates Google Maps API for geocoding and commute calculations, filters properties based on client preferences, and visualizes results on an interactive map using Folium.

### **Features**
- **Dynamic Filtering**: Filter properties based on client preferences such as:
  - Number of bedrooms
  - Price range
  - Location
- **Commute Calculations**: Estimate commute times to a specified destination using Google Maps API.
- **Interactive Visualization**: Display filtered properties on an interactive map with detailed popups showing:
  - Address
  - Price
  - Commute time
- **Batch Processing**: Efficiently processes data in batches to optimize costs with Google Maps API.

---

### **Table of Contents**
- [Overview](#overview)
- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Dependencies](#dependencies)
- [Future Enhancements](#future-enhancements)
- [License](#license)

---

### **Setup**

#### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/real-estate-ai-assistant.git
cd real-estate-ai-assistant
```

#### **2. Set Up a Python Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

#### **3. Install Dependencies**
```bash
pip install -r requirements.txt
```

#### **4. Obtain API Keys**
- **Google Maps API Key**: Create a Google Cloud Project and enable the Geocoding and Distance Matrix APIs.
- Add your API key to a `.env` file:
  ```plaintext
  GOOGLE_MAPS_API_KEY=your_api_key_here
  ```

#### **5. Run the Jupyter Notebook**
Launch the Jupyter Notebook to explore and run the project:
```bash
jupyter notebook
```

---

### **Usage**
1. Open the `Real Estate AI Assistant.ipynb` file in Jupyter Notebook.
2. Update `client_preferences` in the notebook to specify:
   - Number of bedrooms
   - Minimum and maximum price range
   - Preferred location
3. Run all cells to:
   - Process the dataset
   - Filter properties
   - Generate commute times
   - Visualize results on a map
4. View the map directly in the notebook or save it as an HTML file.

---

### **File Structure**
```
real-estate-ai-assistant/
├── data/
│   ├── properties.csv           # Sample dataset of properties
├── Real Estate AI Assistant.ipynb # Jupyter Notebook for the project
├── requirements.txt             # Python dependencies
├── README.md                    # Project documentation
└── .env                         # API keys (not included in Git)
```

---

### **Dependencies**
The following Python libraries are required:
- `folium`: For map visualization
- `pandas`: For data manipulation
- `googlemaps`: For Google Maps API integration
- `python-dotenv`: For securely storing API keys

Install them via:
```bash
pip install -r requirements.txt
```

---

### **Future Enhancements**
- **Property Recommendation**: Suggest properties based on user history or preferences.
- **Advanced Filtering**: Add filters like square footage, property type, or neighborhood rating.
- **Scalability**: Integrate with larger datasets and optimize for performance.
- **Deployment**: Host the app as a web service using Flask or FastAPI.

---

### **License**
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

### **Contributing**
We welcome contributions to enhance this project. Please open an issue or submit a pull request!

---

Zillow Data Set (kaggle): https://www.kaggle.com/datasets/robikscube/zillow-home-value-index
