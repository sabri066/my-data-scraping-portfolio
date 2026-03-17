📊 Book Price Analysis Using Web Scraping

📌 Objective
The goal of this project is to simulate a real-world business scenario where product pricing data is collected from an e-commerce website and analyzed to identify pricing patterns, trends, and distribution. This type of analysis helps businesses make pricing decisions and understand market positioning.
### 📈 Skills Demonstrated

- Web Scraping (requests, BeautifulSoup)
- Data Cleaning (handling encoding issues)
- Data Analysis (pandas)
- Data Visualization (matplotlib)
- Problem Solving (debugging, data formatting)
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
- Average Price: 38.05
- Highest Price: 57.25
- Lowest Price: 13.99
💡 Insights
- The majority of books are priced between £45 and £55, indicating a premium pricing cluster.
- A smaller group of books falls below £25, suggesting discounted or budget offerings.
- The price distribution is slightly right-skewed, meaning more books are concentrated in the higher price range.
- This pricing structure suggests a market strategy focused on mid-to-high value products rather than low-cost volume sales.
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
