Create a folder name *data* in your working directory first.

## Command-Line Usage

### 1. Scraping Business Links

```bash
python script_name.py --keyword "your business keyword" -l
```

- This command scrapes links of businesses based on your keyword and stores them in:
  ```
  data/links/{keyword}.csv
  ```

### 2. Scraping Detailed Business Data

```bash
python script_name.py --keyword "your business keyword" -r
```

- This command uses the links from `data/links/{keyword}.csv` to scrape detailed business information and saves it in:
  ```
  data/{keyword}.csv
  ```

### 3. Folder Structure and Data Usage

- **`data/links/`**: Stores the business profile links in a CSV files.
  - Example: `data/links/Real Estate Firms.csv`
- **`data/`**: Stores the detailed scraped data.
  - Example: `data/Real Estate Firms.csv`

### 4. Running Both Steps Together

First, scrape links:

```bash
python script_name.py --keyword "plumbers" -l
```

Then, scrape details using the saved links:

```bash
python script_name.py --keyword "plumbers" -r
```

## Results
![screencapture-docs-google-spreadsheets-d-1AezDC9mLEjPMWdDLsbyYEdUzc5ylrMxcNFWrNVf3Q8Q-edit-2024-09-15-20_31_05](https://github.com/user-attachments/assets/f723219c-df4d-435c-96ff-b0ba5b75eb99)
