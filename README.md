
# Real-Time Stock Market Scraper

This project automates the process of gathering real-time stock market information. Using Selenium and other Python tools, it scrapes live data, processes it, and provides organized insights for analysis and reporting.

## Features

- Automates login to stock-related websites (if required).
- Scrapes real-time stock market information based on user-defined keywords or stock symbols.
- Cleans and organizes the extracted data for better readability.
- Saves the collected information in formats suitable for further analysis.
- Provides flexibility to add new stock symbols dynamically.

## Requirements

The project uses the following dependencies, which are listed in the `requirements.txt` file:

- `selenium==4.16.0`
- `groq==0.4.2`
- `python-docx==1.1.0`
- `requests==2.31.0`
- `python-dotenv==1.0.0`
- `diffusers==0.25.0`
- `transformers==4.37.2`
- `torch==2.2.0`
- `accelerate==0.26.1`

Install all dependencies using:
```bash
pip install -r requirements.txt
```

## Setup

### Step 1: Clone the Repository
Clone the project repository from GitHub and navigate into the directory:
```bash
git clone https://github.com/yourusername/StockMarketScraper.git
cd StockMarketScraper
```

### Step 2: Install Dependencies
Use the following command to install the required Python libraries:
```bash
pip install -r requirements.txt
```

### Step 3: Configure Environment Variables
1. Create a `.env` file in the project root directory.
2. Add the following environment variables:
   ```
   TWITTER_USERNAME=your_twitter_username
   TWITTER_PASSWORD=your_twitter_password
   GROQ_API_KEY=your_groq_api_key
   HF_API_TOKEN=your_hugging_face_api_token
   CHROMEDRIVER_PATH=path_to_chromedriver
   ```
   Replace placeholders with your actual credentials and paths.

### Step 4: Update ChromeDriver Path
Ensure you have ChromeDriver installed. Update the `PATH` variable in the `stockmarket.py` script with the location of your ChromeDriver.

## How to Use

### Step 1: Run the Script
Launch the program by running the following command in your terminal:
```bash
python stockmarket.py
```

### Step 2: Input Search Terms
You will be prompted to enter the stock-related terms or symbols you want to track. For example:
```
Enter search terms (one per line, press Enter twice to finish):
AAPL
GOOGL
MSFT
```
Press **Enter** twice to start the data scraping process.

### Step 3: Data Extraction
The script will:
1. Log in to the stock market website (if required).
2. Search for real-time stock market data based on the entered terms.
3. Extract, clean, and organize the data.

### Step 4: View Results
The scraped stock market data will be saved in the specified output directory or displayed directly in the terminal. 

## Directory Structure

```
StockMarketScraper/
│
├── stockmarket.py       # Main script to run the scraper
├── requirements.txt     # List of required Python libraries
├── .env                 # Environment variables (not included, create manually)
├── README.md            # Project documentation
└── output/              # Directory where results will be saved
```

## Notes

- Ensure that your `.env` file contains the correct credentials and paths.
- Keep ChromeDriver updated to avoid compatibility issues.
- Use a stable internet connection for uninterrupted execution.
- If the script stops unexpectedly, check the terminal for error messages.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

### Contributors

- **Ajay S**: Developer and maintainer
