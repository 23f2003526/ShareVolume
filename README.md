# Carrier Global Shares Outstanding Web App

## Overview

This web application displays data on Carrier Global Corporation's (CIK 0001783180) common stock shares outstanding, fetched live from the SEC EDGAR API for the concept `EntityCommonStockSharesOutstanding`. It shows the maximum and minimum shares outstanding (post fiscal year 2020) in a visually clear format.

The page dynamically updates if a `?CIK=XXXXXXXXXX` query parameter is present with a different valid 10-digit CIK, fetching and displaying data for that CIK without a page reload.

## Setup

No special setup or dependencies needed. This is a single HTML file that runs entirely in a modern web browser.

## Usage

- Open `index.html` directly in a browser or serve it via a webserver.
- By default, it shows Carrier Global's shares outstanding data.
- To view another company, append a query parameter `?CIK=0001018724` (or any other valid 10-digit CIK) to the URL, e.g.:

  ```
  file:///path/to/index.html?CIK=0001018724
  ```

- The page will fetch via the SEC API or a CORS proxy and update all values and titles accordingly without reloading.

- On initial visit (default CIK), the app will also trigger a download of `data.json` containing the processed data as requested.

## License

MIT License

---

uid.txt (provided separately)