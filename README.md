# Clothing Similarity Finder
This project is aimed at finding similar clothing items based on their descriptions. It scrapes data from several e-commerce websites, processes the data, creates embeddings using a sentence transformer model, and finally provides an API endpoint to find similar clothing items.

## Project Structure
1. Data scraping from ASOS, Flipkart, Zalando, and Macy's.
2. Data cleaning and preprocessing.
3. Text embedding using the SentenceTransformer model.
4. Flask API endpoint that uses cosine similarity to find similar clothing items.

## Requirements
- Python 3.7+
- sentence-transformers
- BeautifulSoup
- pandas
- flask
- nltk
- google-cloud-storage

To install these packages, use pip:

```bash
pip install sentence-transformers beautifulsoup4 pandas flask nltk google-cloud-storage

# Usage
To run the project, execute the Python script:
python ClothingSimillarity.py

To find similar items, make a POST request to the /find-similar-items endpoint with a JSON body containing the item description. Here is an example using curl:
curl -X POST -H "Content-Type: application/json" -d '{"item_description": "your-item-description-here"}' http://localhost:5000/find-similar-items
Contributing
Contributions to this project are welcome! Feel free to submit a Pull Request.
