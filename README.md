# **GitHub Topics & Repositories Scraper**  

A Python-based web scraper that extracts **GitHub topics and their top repositories**, then saves the data into structured CSV files for further analysis.

---

## **📌 Project Overview**
This project **scrapes GitHub Topics** from the [GitHub Topics Page](https://github.com/topics) and retrieves information about **top repositories** under each topic.  
The scraped data is then **saved as CSV files** inside the `Data/` directory.

---

## **🛠 Tools Used**
This project was built using the following technologies:  
- **Python** - The core programming language  
- **BeautifulSoup** - For parsing and extracting HTML data  
- **Requests** - To send HTTP requests and fetch web pages  
- **Pandas** - For data manipulation and exporting to CSV  

---

## **🔍 Features**
- Extracts a list of top **GitHub topics** (Machine Learning, Data Science, etc.)
- Retrieves **top repositories** under each topic
- Extracts **repository details** (username, repo name, stars, repo URL)
- Saves all data into **CSV files** for easy analysis
- Implements **logging** to track scraping progress and errors

---

## **📂 Project Structure**
```
├── GitHub_Scraper.ipynb    # Jupyter Notebook containing the scraper
├── LOGS/                   # Stores log files for debugging
├── Data/                   # Stores CSV files with scraped data
└── README.md               # Project documentation
```

## **⚙️ How It Works**
1. **Scrape GitHub Topics** - The script fetches the top topics from GitHub and extracts their names, descriptions, and URLs.  
2. **Scrape Top Repositories** - For each topic, the script scrapes **top repositories**, extracting details like **username, repo name, star count, and repo URL**.  
3. **Save Data to CSV** - Extracted data is stored in structured **CSV files**, one for each topic.  
4. **Logging for Debugging** - A logging system is implemented to track the scraping progress and handle errors.  

---

## **📊 Example Output**
Example **3D** topic data stored in `Data/3d.csv`:

![Example CSV Screenshot](https://github.com/user-attachments/assets/d949f6e8-e2e2-44fd-b848-cf2a45e79214)

---

## **🔧 Setup & Installation**
### **1. Clone the Repository**
```sh
git clone https://github.com/Shruti-H/github-topic-repo-scraper.git
cd github-topic-repo-scraper
```

### **2. Open Jupyter Notebook**
```sh
jupyter notebook scraping-github-topics-repositories.ipynb
```
*If Jupyter Notebook is not installed, install it using:*
```sh
pip install notebook
```

### **3. Run the Notebook**
- Open `scraping-github-topics-repositories.ipynb` in Jupyter Notebook.
- Click **"Run All"** to execute all the cells.

---

## **🚀 Future Work**
- Further analyze CSV data using **Pandas, SQL, or visualization tools**.
- Improve scraping speed using **parallel processing**.
- Add **database storage** for structured data retrieval.
- Extract additional repository details (Forks, Issues, Contributors).
- Implement **pagination** to scrape **more topics and repositories** by iterating through multiple pages (`?page=1`, `?page=2`, etc.).

---
