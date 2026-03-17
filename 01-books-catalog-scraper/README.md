📊 Book Price Analysis Using Web Scraping

📌 Objective

This project extracts and analyzes book pricing data from an online catalog to understand pricing trends and distribution.

## Website Scraped
[http://books.toscrape.com/](http://books.toscrape.com/) – a safe practice site.

🛠 Tools Used
- Python
- requests
- BeautifulSoup
- pandas
- matplotlib

## Process
🔄 Process
1. Scraped book titles and prices from website
2. Cleaned price data by removing encoding issues
3. Converted prices into numeric format
4. Performed statistical analysis
5. Visualized price distribution

📊 Key Results
- Average Price: 38.048500000000004
- Highest Price: 57.25
- Lowest Price: 13.99
💡 Insights
- Most books fall within a mid-range price
- A few books are priced significantly higher
- Price distribution shows variation across products
## Output
The resulting CSV file contains 20 rows (one per book) with two columns: `Book Title` and `Price (UK Pounds)`.

## Sample Data Preview
| Book Title | Price |
|------------|-------|
| A Light in the Attic | £51.77 |
| Tipping the Velvet | £53.74 |
| Soumission | £50.10 |
| ... | ... |

## Files in This Folder
- `book_price_analysis.ipynb` – Jupyter/Colab notebook with the code.
- `book_price_analysis.csv` – The final data file.

## How to Run
1. Open the notebook in Google Colab or Jupyter.
2. Run all cells.
3. The CSV file will be generated in the same folder.
