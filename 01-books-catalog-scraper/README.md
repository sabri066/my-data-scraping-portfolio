# Project 1: Book Catalog Scraper

## Objective
The goal of this project was to extract product information from an online bookstore's catalog page. This simulates a real-world task where a client needs product data for analysis.

## Website Scraped
[http://books.toscrape.com/](http://books.toscrape.com/) – a safe practice site.

## Tools Used
- Python 3
- `requests` – to fetch the webpage
- `BeautifulSoup` (bs4) – to parse HTML
- `pandas` – to organize and export data

## Process
1. **Fetch** the webpage using `requests.get()`.
2. **Parse** the HTML content with BeautifulSoup.
3. **Identify** the HTML structure using browser Developer Tools (Inspect).
4. **Find** all book containers (`<article class="product_pod">`).
5. **Extract** title (from `<h3><a title="...">`) and price (from `<p class="price_color">`).
6. **Store** data in Python lists.
7. **Create** a pandas DataFrame.
8. **Export** to CSV file.

## Key Challenges & Solutions
- **Challenge:** Understanding which HTML tags contain the needed data.  
  **Solution:** Used browser Inspect tool to explore the structure.
- **Challenge:** Handling missing data.  
  **Solution:** The site is clean; for practice, I added checks for future robustness.

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
- `books_scraper.ipynb` – Jupyter/Colab notebook with the code.
- `my_first_scraped_books.csv` – The final data file.

## How to Run
1. Open the notebook in Google Colab or Jupyter.
2. Run all cells.
3. The CSV file will be generated in the same folder.
