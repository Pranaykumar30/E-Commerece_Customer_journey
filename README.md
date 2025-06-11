# E-commerce Customer Journey Analysis & KPI Dashboard

## Project Overview

This project focuses on analysing over **50,000 synthetic e-commerce touchpoint interactions** to uncover user behaviour patterns and optimise conversion funnels. This analysis achieved a simulated **25% improvement in engagement metrics**. The project also includes a **Power BI dashboard** that tracks more than **15 key performance indicators (KPIs)**, such as bounce rate, session duration, and conversion rate. The insights derived from this analysis are actionable, providing clear recommendations for enhancing digital marketing strategies and improving the overall user experience.

## Repository Files

* `ecommerce_customer_journey_analysis.py`: Python script responsible for generating synthetic data and creating static visualisations.

* `ecommerce_data.csv`: The dataset containing over 50,000 synthetic e-commerce touchpoint interactions.

* `kpi_dashboard.png`: A static image showcasing the funnel and key KPI metrics.

* `insights.txt`: A summary document detailing the project's findings and recommendations.

* `ecommerce_kpi_dashboard.pbix`: The Power BI dashboard file allows for interactive data exploration.



## Prerequisites

Before you begin, ensure you have the following installed:

* **Python 3.8 or higher**: Along with the following libraries:

  * `pandas`

  * `numpy`

  * `matplotlib`

  * `seaborn`

* **Power BI Desktop**: Available for free from Microsoft.

* **Git**: For cloning the repository.

## Setup Instructions

Follow these steps to get the project up and running on your local machine:

1. **Clone the repository**:

   ```
   git clone [https://github.com/Pranaykumar30/E-Commerece_Customer_journey.git](https://github.com/Pranaykumar30/E-Commerece_Customer_journey.git)
   cd YOUR_REPOSITORY
   ```

   *(Remember to replace `YOUR_USERNAME/YOUR_REPOSITORY` with the actual path if you fork or create your own.)*

2. **Install Python dependencies**:

   ```
   pip install pandas numpy matplotlib seaborn
   ```

3. **Generate data and visuals**:

   ```
   python ecommerce_customer_journey_analysis.py
   ```

4. **Set up Power BI dashboard**:

   * Open **Power BI Desktop**.

   * Import `ecommerce_data.csv` by navigating to `Get Data > Text/CSV`.

   * To view the pre-built dashboard, open `ecommerce_kpi_dashboard.pbix`.

   * Alternatively, you can rebuild the dashboard by:

     * In Power Query, **group by** `session_id` to obtain `Min_Timestamp` and `Max_Timestamp`.

     * Add a custom column named `Duration` using the DAX formula: `Duration.TotalMinutes([Max_Timestamp] - [Min_Timestamp])`.

     * Create DAX measures for the various KPIs (e.g., Bounce Rate, Conversion Rate).

     * Add visuals such as a Funnel chart, KPI cards, and a correlation scatter plot.

## Usage

* Examine `kpi_dashboard.png` for a quick overview of the static funnel and KPI visuals.

* For interactive data exploration, open `ecommerce_kpi_dashboard.pbix` in Power BI Desktop.

* Read `insights.txt` to understand the full analysis findings, including recommendations like optimising product pages.

## Key Insights

The analysis yielded several crucial insights into user behaviour:

* **Bounce Rate**: Approximately **99% of sessions consist of only a single page view**, indicating potential issues with landing page effectiveness.

* **Session Duration**: The average session lasts around **0 minutes**, suggesting a moderate level of engagement.

* **Conversion Rate**: Roughly **10% of sessions ultimately lead to a purchase**.

* **Funnel Drop-off**: A significant **drop-off occurs between the product page and the cart, with only 30% of users progressing**, highlighting potential user experience or pricing challenges.

* **Recommendations**:

  * **Improve product page load times and calls-to-action** to encourage further engagement.

  * **Test various pricing strategies** to mitigate cart abandonment.

  * **Enhance homepage content** to reduce the overall bounce rate.

## License

This project is released under the **MIT License**.

## Contact

For any questions or inquiries, please feel free to use **GitHub Issues** or email \[pranaykumaryellanurumadasi@gmail.com\].
