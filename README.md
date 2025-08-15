# 📊 Web Scraping Dashboard

An interactive **Jupyter Notebook Dashboard** for scraping real-world data on **Weather**, **News**, and **Cryptocurrency**.
---

## 🚀 Features

* **Weather Data** 🌤

  * Live temperatures for major cities (London, New York, Tokyo, Delhi, Sydney).
  * Bar chart visualization.
  * Download as `weather.csv`.

* **News Headlines** 📰

  * Choose category: *General, Sports, Environment, Social Trends*.
  * Shows top 15 headlines.
  * Word frequency bar chart.
  * Download as `news_<topic>.csv`.

* **Cryptocurrency Prices** 💰

  * Top 5 cryptocurrencies (by market cap) from CoinGecko API.
  * Bar chart of prices in USD.
  * Download as `crypto.csv`.

* **All Data Option** 📦

  * Scrapes Weather, News, and Crypto together.
  * Saves all CSVs into `all_data.zip`.
  * Single download link.

### 2. Install dependencies

Run the following in your terminal or Jupyter cell:

```bash
pip install requests beautifulsoup4 pandas matplotlib ipywidgets
```

For **Jupyter Notebook (classic)**, enable widgets:

```bash
!jupyter nbextension enable --py widgetsnbextension
```

## ▶️ Usage

1. Open the notebook:

```bash
jupyter notebook webscraping_dashboard.ipynb
```

2. Run all cells.

3. Use the dropdown to select:

   * **Weather**
   * **News** (then select *General, Sports, Environment, Social Trends*)
   * **Cryptocurrency**
   * **All Data**

4. View scraped results in table + chart.
---

## 📂 Output Files

* `weather.csv` → Weather data
* `news_<topic>.csv` → News headlines for the chosen topic
* `crypto.csv` → Cryptocurrency prices
* `all_data.zip` → Bundle of all datasets

---

## ⚠️ Notes

* News scraping depends on BBC’s current page structure. If headlines fail, update the CSS selector (`h3`).
* Weather scraping uses [wttr.in](https://wttr.in) free API.
* Cryptocurrency data comes from the [CoinGecko API](https://www.coingecko.com).

--
