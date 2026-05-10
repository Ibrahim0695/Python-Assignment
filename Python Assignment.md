# Python Data Fetching & CSV Export Assignment

## Overview

This Jupyter notebook fetches data from three different JSON API sources, converts them into pandas DataFrames, and exports them as CSV files for further analysis.

## Data Sources

| Source | URL | Description |
|--------|-----|-------------|
| Mock Data | `https://raw.githubusercontent.com/Ibrahim0695/mock_data/.../MOCK_DATA.json` | 105 records of user data (names, emails, genders, IPs) |
| Products | `https://dummyjson.com/products` | 30 products with categories, pricing, stock, reviews |
| Carts | `https://dummyjson.com/carts` | 30 shopping carts with product line items, totals, user IDs |

## Workflow

1. **Fetch** — Uses `requests.get()` to pull JSON data from each endpoint
2. **Parse** — Converts JSON responses to Python dicts/lists via `.json()`
3. **DataFrame** — Creates pandas DataFrames from the parsed data
4. **Export** — Saves each DataFrame as a CSV file

## Output Files

| File | Contents |
|------|----------|
| `mock_data.csv` | Raw user mock data (105 rows) |
| `p_data.csv` | Products data with 22 columns (id, title, price, category, etc.) |
| `c_data.csv` | Carts data with 7 columns (id, products, total, userId, etc.) |

## Requirements

- `requests`
- `pandas`

## Usage

Open the notebook in Jupyter or Google Colab and run all cells. The CSV files will be generated in the working directory.
