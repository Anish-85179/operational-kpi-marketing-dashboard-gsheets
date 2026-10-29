# Operational KPI & Marketing Metric Board

An executive-grade, multi-channel marketing performance and operational KPI analytics console built natively in Google Sheets. Designed with an Apple-grade clean light-mode aesthetic (`#FFFFFF` canvas), this workbook transforms raw marketing transactions into interactive, real-time executive intelligence.

---

## 🏗️ Workbook Architecture

The workbook is structured into 4 optimized, interconnected sheets:

1. **`Raw_Data`**
   * **Purpose:** Ingestion layer containing 100 enterprise marketing campaign transaction records.
   * **Metrics Tracked:** Campaign ID, Date, Channel, Campaign Name, Impressions, Clicks, Spend (`USD`), Conversions, Revenue (`USD`), and automated ROAS (`=Revenue/Spend`).

2. **`Pivot_Engine`**
   * **Purpose:** Calculation and aggregation backend.
   * **Features:** Groups metrics by marketing channel using robust `SUMIF` formulas and error-handling functions (`IF`) to ensure fault-tolerant ROAS calculations.

3. **`Dashboard`**
   * **Purpose:** Executive command center.
   * **Layout:** Top-line KPI summary blocks (Total Spend, Total Revenue, Blended ROAS, Total Conversions), linked summary tables, embedded column visualizations, and interactive **Channel Slicers** for real-time multi-criteria filtering.

4. **`Lookup_Reference`**
   * **Purpose:** Metadata reference repository.
   * **Contents:** Channel target benchmarks, maximum monthly budget caps, and campaign manager assignments with professional light-mode formatting.

---

## 🛠️ Core Formulas & Logic
* **Blended ROAS Calculation:**
  ```sheets
  =IF(A6=0, 0, C6/A6)
* **Blended ROAS Calculation:**
  ```sheets
  =IF(A6=0, 0, C6/A6)
