 E-commerce Behavior Analysis

Summary
-------
This repository contains an end-to-end exploratory analysis and segmentation workflow for the Olist e-commerce dataset. The primary analysis is implemented in `book1.ipynb` and covers data cleaning, geolocation visualizations, RFM & CLV segmentation, product ABC analysis, time-series GMV forecasting, and seller evaluation.

Quick start
-----------
1. Clone the repository.
2. Place required CSVs in the project root (or `data/`) and add a valid Mapbox token to `mapbox_token.txt`.
3. Create a virtual environment and install 
python -m venv .venv .venv\Scripts\activate pip install -r requirements.txt
4. Open `book1.ipynb` in Jupyter or PyCharm and run cells sequentially.

Required data files
-------------------
Place these CSV files in the project root or `data/`:
- `olist_geolocation_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_order_payments_dataset.csv`
- `olist_order_reviews_dataset.csv`
- `olist_orders_dataset.csv`
- `olist_products_dataset.csv`
- `olist_sellers_dataset.csv`
- `product_category_name_translation.csv`
- `olist_customers_dataset.csv`

Mapbox token
------------
- Add a Mapbox access token in `mapbox_token.txt` (single line). Keep this file out of version control (add to `.gitignore`) if the token is private.

Environment & dependencies
--------------------------
- Python 3.8+ (Windows)
- Core packages used: `pandas`, `numpy`, `plotly`, `matplotlib`, `seaborn`, `folium`, `geopy`, `scikit-learn`, `shap`
- Install with `pip install -r requirements.txt`

How to run
----------
- Open `book1.ipynb` in Jupyter Notebook / JupyterLab or run in PyCharm Notebook mode.
- Execute cells in order. Interactive Plotly charts render in a notebook; if working offline, export static images via Plotly / Matplotlib and save them to `docs/images/`.

Saved images & embedded previews
--------------------------------
Place generated images in `docs/images/`. Example image names used in the notebook and README:

- `docs/images/top10_locations.png` — Top 10 selling locations
- `docs/images/customer_map.png` — Customer scattermap
- `docs/images/state_choropleth.png` — Spending by state (choropleth)
- `docs/images/new_returning_monthly.png` — New vs returning customers (monthly)
- `docs/images/clv_segmentation.png` — CLV segmentation
- `docs/images/rfm_segmentation.png` — RFM segmentation
- `docs/images/top_product_categories.png` — Product categories (bar + GMV)
- `docs/images/abc_pareto.png` — Product ABC pareto
- `docs/images/volatility_plot.png` — Product volatility
- `docs/images/daily_gmv.png` / `docs/images/monthly_gmv.png` — Time-series GMV
- `docs/images/actual_vs_predicted.png` — Forecast comparison
- `docs/images/review_histogram.png` — Review score distribution
- `docs/images/seller_suggestion.png` — Seller recommendation snapshot

Embedded previews (rendered by viewers that support images):
![Top 10 selling locations](/docs/images/top10_locations.png)
![Customer map](/docs/images/customer_map.png)
![Spending by state](/docs/images/state_choropleth.png)

Project layout
--------------
- `book1.ipynb` — Main analysis notebook
- `requirements.txt` — Python dependencies
- `docs/images/` — Saved images referenced by the notebook / README
- CSV data files — project root or `data/`
- `mapbox_token.txt` — Mapbox access token

Notes & tips
-----------
- Keep `mapbox_token.txt` private or add to `.gitignore`.
- If interactive renderers fail, save static figures to `docs/images/` and view them from the README.
- Update image filenames in README if your saved images use different names.

Author
------
Created by Cyrus

License
-------
MIT
