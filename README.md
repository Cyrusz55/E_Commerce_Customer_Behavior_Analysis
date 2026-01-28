🛒 E-commerce Behavior Analysis (Olist Dataset)


An end-to-end data analytics & customer intelligence project built on the Brazilian Olist e-commerce dataset, covering exploratory analysis, customer segmentation, forecasting, and seller evaluation.


📊 Focus: turning raw transactional data into business-driven insights



---

🔍 Project Highlights


✅ End-to-end data pipeline (raw CSV → insights)

✅ Customer segmentation using RFM & CLV

✅ Geospatial analysis with Mapbox & Plotly

✅ Product performance via ABC / Pareto analysis

✅ GMV time-series forecasting

✅ Seller performance evaluation & recommendations


---

📂 Project Structure

	.
	├── book1.ipynb                # Main analysis notebook
	├── requirements.txt           # Python dependencies
	├── mapbox_token.txt           # Mapbox access token (gitignored)
	├── data/                       # Raw CSV datasets (optional)
	├── docs/
	│   └── images/                # Generated plots & figures
	└── README.md


---

📊 Key Visualizations (Previews)
<p align="center">
  <img src="docs/images/top_15_Selling_products%20categories.png" width="45%">
  <img src="docs/images/top_10%20selling_loc.png" width="45%">
</p><p align="center">
  <img src="docs/images/monthly%20gmv.png" width="60%">
</p>
---

🧠 Analyses Performed

Customer Analytics

- RFM segmentation (Recency, Frequency, Monetary)

- CLV estimation & customer value tiers

- New vs. returning customer trends

Product Analytics

- Top categories by GMV

- ABC / Pareto classification

- Demand volatility analysis

Sales & Forecasting

- Daily & monthly GMV time series

- Forecast vs. actual comparison

- Trend & seasonality insights

Seller Evaluation

- Review score distribution

- Performance benchmarking

- Seller recommendation logic


---

🚀 Quick Start

1️⃣ Clone the Repository

	git clone https://github.com/your-username/ecommerce-behavior-analysis.git
	cd ecommerce-behavior-analysis

2️⃣ Add Required Data


Place the following CSV files in the project root or data/ directory:


- olist_orders_dataset.csv

- olist_order_items_dataset.csv

- olist_order_payments_dataset.csv

- olist_order_reviews_dataset.csv

- olist_customers_dataset.csv

- olist_products_dataset.csv

- olist_sellers_dataset.csv

- olist_geolocation_dataset.csv

- product_category_name_translation.csv

3️⃣ Environment Setup

	python -m venv .venv
	.venv\Scripts\activate
	pip install -r requirements.txt

4️⃣ Mapbox Configuration


Create a file called mapbox_token.txt and paste your Mapbox token (single line).


⚠️ Keep this file private and add it to .gitignore


5️⃣ Run the Notebook


Open book1.ipynb in:


- Jupyter Notebook / JupyterLab


- PyCharm (Notebook mode)

Run cells sequentially.


---

🖼️ Generated Outputs


All figures are saved to docs/images/ and referenced in the notebook and README.

Examples:


- rfm_segmentation.png

- clv_segmentation.png

- abc_pareto.png

- daily_gmv.png

- actual_vs_predicted.png

- seller_suggestion.png


---

🛠️ Tech Stack

- Language: Python 3.8+

- Data: Pandas, NumPy

- Visualization: Plotly, Matplotlib, Seaborn, Folium

- Geo: Mapbox, Geopy

- ML / Analytics: Scikit-learn, SHAP


---

📌 Notes

- Interactive Plotly charts work best inside notebooks.

- For static viewing (GitHub), export figures to docs/images/.

- Update README image paths if filenames change.


---

👤 Author


Cyrus

Engineer | Data Analyst | Math & ML Enthusiast


---

📄 License


MIT License


---

✅ Optional Enhancements (Tell me if you want these)

- Add Business Insights & Recommendations section


- Add Model assumptions & limitations


- Convert notebook → portfolio-ready HTML report

- Add badges (Python, License, Notebook, Dataset)