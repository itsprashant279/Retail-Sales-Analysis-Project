## 📊 Dataset Overview

The primary dataset, `P_1_retail_sales_dataset.xlsx`, contains 1,000 transaction records capturing retail sales data across a one-year period. 

### Core Features (Columns):
*   **Transaction ID**: Unique identifier for each sale.
*   **Date**: The date the transaction took place.
*   **Customer ID**: Unique identifier for the customer.
*   **Gender**: Customer's gender (Male/Female).
*   **Age**: Age of the customer.
*   **Product Category**: Industry vertical of the purchased item (`Beauty`, `Clothing`, `Electronics`).
*   **Quantity**: Number of items purchased in the transaction.
*   **Price per Unit**: Cost of a single item.
*   **Total Amount**: Total revenue generated from the transaction ($Quantity \times Price\ per\ Unit$).

---

## 🗂️ Workbook Structure

The Excel file `P_1_retail_sales_dataset.xlsx` is divided into structured sheets, breaking down the analytical pipeline from raw data to insights:

| Sheet Name | Description |
| :--- | :--- |
| `retail_sales_dataset` | The raw, cleaned transactional dataset used as the single source of truth. |
| `Descriptive_statistics`| High-level summary statistics calculating data distribution, averages, totals, and standard deviations. |
| `Time-series analysis` | Sales trends tracking revenue growth, transaction volume, and seasonality month-over-month. |
| `Customer_analysis` | Segmentations exploring demographic breakdowns (age brackets and gender) relative to purchasing habits. |
| `Product_analysis` | Matrix evaluating performance, total items sold, and revenue generated per product category. |
| `Visualization` | Clean dashboard layouts featuring charts and pivot tables for stakeholders. |

---

## 🔑 Key Insights Addressed

1. **Demographic Focus:** Identifying which age groups and genders drive the majority of the revenue.
2. **Product Performance:** Tracking which product categories yield the highest transaction volume vs. overall revenue margins.
3. **Temporal Trends:** Pinpointing peak sales months or seasonal spikes to optimize inventory and marketing spend.

---

## 🚀 Getting Started

### Prerequisites
To explore or modify the workbook, you will need:
*   Microsoft Excel (2016 or newer) or Google Sheets.
*   *(Optional)* Python (with `pandas` and `openpyxl`) if you plan to automate further analysis.

### Quick Python Code snippet to inspect the data:
```python
import pandas as pd

# Load the core dataset
file_name = "P_1_retail_sales_dataset.xlsx"
df = pd.read_excel(file_name, sheet_name="retail_sales_dataset")

# Display basic info
print(df.info())
print(df.head())
