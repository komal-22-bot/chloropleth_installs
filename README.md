# Interactive Choropleth Map: Global Installs by App Category

This project displays a dynamic, interactive Choropleth map using Plotly and Streamlit to visualize app installs across different countries and categories, with a twist — it only works during a specific time window.

**Time Restriction Logic (IST)**
This visualization is restricted to display only between 6 PM and 8 PM IST. Outside of this window, the dashboard will show a message like:
*Visualization is only available between 6 PM and 8 PM IST.*

**Tech Stack**
-Python
-Plotly
-Pandas
-Dash (for dashboard integration)
-DateTime (for time filtering)

## Features

- Visualize **global app installs** by category.
- Only shows data for **Top 5 categories** (based on install count).
- Filters out app categories starting with **A, C, G, or S**.
- Highlights categories with installs exceeding **1 million**.
- Map is visible **only between 6 PM and 8 PM IST** for controlled access.

## Logic Behind

- **Data Filtering**:
  Excludes certain starting characters and limits to top 5.
- **Time Restriction**:
  Uses `datetime` and `pytz` to enforce time-based visibility.
- **Visualization**:
  Built with Plotly's Choropleth features and integrated into a Streamlit app.

 **License**
This project is open-sourced under the MIT License. 
