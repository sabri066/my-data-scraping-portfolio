# Project 2: Famous Quotes Scraper

## Objective
This project practices adapting a scraper to a new website. The task was to collect famous quotes and their authors from a practice quotes site.

## Website Scraped
[http://quotes.toscrape.com/](http://quotes.toscrape.com/) – a safe practice site.

## Tools Used
- Python 3
- `requests` and `BeautifulSoup` for scraping
- `pandas` for data export

## Process
1. **Inspected** the website using Developer Tools to find the HTML structure.
2. **Identified** the quote container: `<div class="quote">`.
3. **Located** quote text inside `<span class="text">` and author inside `<small class="author">`.
4. **Modified** the original books scraper code to target these new elements.
5. **Extracted** all quotes from the first page (10 items).
6. **Saved** to CSV.

## Key Learning
- How to **inspect and adapt** code to a new site.
- Understanding that the **same scraping pattern** (find container → find elements inside) applies to any site.
- The importance of `.text` to get clean content.

## Output
CSV file with two columns: `Quote` and `Author`.

## Sample Data Preview
| Quote | Author |
|-------|--------|
| “The world as we have created it is a process of our thinking...” | Albert Einstein |
| “It is our choices, Harry, that show what we truly are...” | J.K. Rowling |
| ... | ... |

## Files in This Folder
- `quotes_scraper.ipynb` – Notebook with the code.
- `my_first_scraped_quotes.csv` – The final data file.

## How to Run
1. Open in Google Colab or Jupyter.
2. Run all cells.
3. The CSV file will be created.
