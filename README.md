
# AI Web Scraping App

This web application allows users to scrape data from any website by simply providing a URL. It uses Selenium, BrightData, and Ollama AI to interact with and analyze the scraped data. After scraping, you can ask the integrated AI specific questions about what data you need from the website.

## Features
- **Web Scraping**: Provide a URL, and the app will scrape the data from the website using BrightData.
- **Data Cleaning**: The scraped data is cleaned and processed for further analysis.
- **AI Interaction**: The app integrates Ollama AI, allowing you to ask specific questions about the data, like what to scrape and how to use it.

## Technologies Used
- **Selenium**: Automates the web scraping process.
- **BrightData**: Used for large-scale scraping instead of local scraping.
- **Ollama AI**: For processing and interacting with the scraped data.
- **Python**: The main programming language used to build the app.
- **BeautifulSoup**: For parsing and cleaning the HTML data.

## Prerequisites
Before running the project, ensure you have the following installed:
- **Python 3.x**
- **pip** (Python package installer)
- **BrightData account**: For using their scraping services. [BrightData Documentation](https://brightdata.com/)
- **Selenium**: Install it via pip (`pip install selenium`).
- **Ollama**: Make sure you have access and API keys for Ollama.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up environment variables:
   - Create a `.env` file in the root directory and add your environment variables:
     ```env
     SBR_WEB_DRIVER=<path_to_your_web_driver>
     BRIGHT_DATA_API_KEY=<your_brightdata_api_key>
     OLLAMA_API_KEY=<your_ollama_api_key>
     ```

4. Download the appropriate web driver for Selenium (e.g., `chromedriver`) and add its path to the `.env` file.

## Usage

1. **Start the Web App**:
   ```bash
   python main.py
   ```

2. **Scrape a Website**:
   - Input the URL of the website you want to scrape into the app.

3. **Ask the AI**:
   - After scraping, use Ollama AI to ask what specific data you need from the website, and the app will provide the requested information.

## Example

1. Run the app:
   ```bash
   python main.py
   ```

2. Provide the URL to scrape (e.g., https://example.com).

3. Interact with the AI:
   - You can ask, "Extract all the product names from the page" or "Give me all the contact information from the page," and Ollama will process the request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
