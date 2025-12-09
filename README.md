## 📊 Dashboard Overview

This interactive dashboard provides real-time insights into sales performance, profitability, shipments, and operational metrics for a chocolate manufacturing and distribution company.

### 📱 Dashboard Views

The dashboard consists of four main views, each providing unique analytical perspectives:

#### 1️⃣ **Salesperson Performance Dashboard**
![Salesperson Dashboard](<Salesperson Performance Dashboard.png>)

**Focus**: Individual sales team member analysis
- **Primary Table**: Salesman, Team, Sales, Profit, LBS_Ratio, Profit_Ratio
- **Use Case**: Identify top performers, track team contributions, monitor individual quotas
- **Key Insights**: Performance rankings, team comparisons, commission calculations
- **Visual Indicators**: Checkmarks (✓) for high performers, warning icons (🟠) for attention areas

#### 2️⃣ **Product Analytics Dashboard**
![Product Dashboard](<Product Analytics Dashboard.png>)

**Focus**: Product-level profitability and performance
- **Primary Table**: Product, Category, Sales, Profit, LBS_Ratio, Profit_Ratio
- **Use Case**: Product portfolio optimization, inventory decisions, pricing strategy
- **Key Insights**: Best-selling products, profit margins by item, category performance
- **Categories**: Bars, Bites, Other
- **Products Include**: White Choc, Spicy Special Slims, Smooth Silky Salty, Raspberry Choco, Peanut Butter Cubes, and more

#### 3️⃣ **Geographic Sales Dashboard**
![Geographic Dashboard](<Geographic Sales Dashboard.png>)

**Focus**: Country-wise sales distribution and market analysis
- **Primary Visual**: Interactive pie chart showing sales by countries
- **Countries Analyzed**: 
  - 🇮🇳 India
  - 🇬🇧 UK
  - 🇨🇦 Canada
  - 🇺🇸 USA
  - 🇦🇺 Australia
  - 🇳🇿 New Zealand
- **Use Case**: Market penetration analysis, geographic expansion planning, regional performance tracking
- **Key Insights**: Market share by country, revenue distribution, growth opportunities

#### 4️⃣ **Country-Filtered Dashboard** (Australia Example)
![Country-Filtered Dashboard](<Country-Filtered Dashboard.png>)

**Focus**: Deep-dive analysis for specific markets
- **Example**: Australia market view
- **Filtered Metrics**:
  - Sales: $3,385K (12.7% ↓ MoM)
  - Profit: $1,505K (4.1% ↓ MoM)
  - Shipments: 577 (3% ↓ MoM)
  - Boxes: 292K (3% ↓ MoM)
  - LBS_Count: 28 (100% ↑ MoM)
  - Profit Ratio: 44.5%
- **Use Case**: Country-specific strategy, localized reporting, market-specific insights
- **Capability**: Demonstrates dynamic filtering - select any country to view its isolated performance

## ✨ Key Features

### 📈 Dynamic Visualizations

1. **Interactive Line Charts**
   - Tracks monthly trends for Sales, Profit, Shipments, and LBS_Count
   - Button slicer to switch between different metrics
   - Displays data from January 2023 to July 2024
   - Clear visualization of performance peaks and valleys

2. **Shipment Distribution Analysis**
   - Stacked column chart showing total shipments by bins (50 boxes)
   - Range: 0-50 boxes per shipment
   - Helps identify optimal shipment sizes and distribution patterns

3. **Performance Gauges**
   - **Profit Ratio Gauge**: Displays overall profit margin percentage
   - **LBS Ratio Gauge**: Shows LBS efficiency metric
   - Quick visual indicators of key performance metrics
   - Color-coded ranges (red, yellow, green) for performance assessment

### 📋 KPI Cards

Five comprehensive KPI cards displaying:
- **Sales**: Total sales value with MoM percentage change
- **Profit**: Total profit with MoM percentage change
- **Shipments**: Total number of shipments with MoM growth
- **Boxes**: Total boxes shipped with MoM change
- **LBS_Count**: Total LBS count with MoM percentage

Each card includes:
- Current month value
- Month-over-Month (MoM) percentage change
- **Conditional Color Coding** based on performance criteria:
  - 🟢 **Green (Latest Month)**: Criteria met successfully
  - 🟠 **Orange (MoM%)**: Criteria partially met or approaching target
  - 🔴 **Red (MoM%)**: Criteria not met - requires attention

**Example**: In the Australia-filtered dashboard (Image 4), you can observe red color in MoM(%) indicators. This occurs because the performance metrics don't meet the predefined criteria. When criteria are met, the system displays:
- Orange color for MoM(%) when approaching targets
- Green color for Latest Month values when goals are achieved
- Red color indicates underperformance and the need for corrective action

### 📊 Dynamic Data Tables

**Toggle Between Two Views:**

1. **Salesman Performance Table**
   - Columns: Salesman, Team, Sales, Profit, LBS_Ratio, Profit_Ratio
   - Tracks individual salesperson performance
   - Sortable by any metric
   - Visual indicators for top performers

2. **Product Performance Table**
   - Columns: Product, Category, Sales, Profit, LBS_Ratio, Profit_Ratio
   - Analyzes product-level performance
   - Identifies best and worst performing products
   - Category-wise breakdown (Bars, Bites, Other)

Both tables include:
- Checkmark indicators (✓) for high performers
- Warning indicators (🟠) for attention areas
- Visual bar charts for quick comparison

### 🌍 Geographic Analysis

**Interactive Pie Chart (Tooltip Integration)**
- Embedded as a tooltip in the line chart
- Shows sales distribution across countries:
  - 🇮🇳 India: $611K (25.03%)
  - 🇬🇧 UK: $628K (25.74%)
  - 🇨🇦 Canada: $386K (15.81%)
  - 🇺🇸 USA: $323K (13.2%)
  - 🇦🇺 Australia (shown in charts)
  - 🇳🇿 New Zealand (shown in charts)
- Hover over the line chart to view country-wise breakdown

### 🔧 Interactive Filters

**Four Button Slicers for Dynamic Filtering:**

1. **Year Filter**
   - Options: 2023, 2024
   - Filter all visuals by year

2. **Order Status**
   - Cancelled
   - Delivered
   - Placed
   - Track order lifecycle

3. **Category**
   - Bars
   - Bites
   - Other
   - Product category analysis

4. **Countries**
   - Australia
   - Canada
   - India
   - And more...
   - Geographic filtering

## 🎯 Use Cases

- **Executive Dashboard**: Quick overview of business health and KPIs
- **Sales Analysis**: Track salesperson and product performance
- **Inventory Management**: Monitor shipment patterns and box distribution
- **Strategic Planning**: Identify growth opportunities and underperforming areas
- **Geographic Expansion**: Analyze country-wise sales performance
- **Product Strategy**: Determine which products drive the most profit

## 📁 Data Structure

The dashboard uses data from `Choco Company Data.xlsx` with the following key fields:
- Sales, Profit, Shipments
- Boxes, LBS_Count, LBS_Ratio, Profit_Ratio
- Salesman, Team, Product, Category
- Countries, Order_Status
- Date/Time dimensions for trend analysis

## 🛠️ Technical Implementation

### Power BI Features Used:
- **DAX Measures**: Custom measures for dynamic calculations including:
  - Latest month metrics
  - Month-over-Month percentage calculations
  - Aggregations and ratios
- **Conditional Formatting**: 
  - Color-coded KPI cards with criteria-based formatting
  - Red: Performance below criteria threshold
  - Orange: Performance approaching criteria
  - Green: Performance meeting or exceeding criteria
- **Bookmarks**: Toggle between Salesman and Product views
- **Tooltips**: Interactive country breakdown on hover
- **Button Slicers**: Clean, modern filtering experience
- **Color Coding**: Dynamic color system for performance monitoring

### Key DAX Measures:

#### Latest Month Sales Calculation
```dax
M_Latest_Month_Sale = 
  VAR latest_month = [M_Latest_Month]
RETURN
    CALCULATE([M_Total_Sales], D_Calendar[Start of Month] = latest_month)
```
**Purpose**: Captures sales value for the most recent month in the dataset

#### Month-over-Month Sales Percentage
```dax
M_MOM_Sales_(%) = 
    VAR td = [M_Latest_Month]
    VAR tms = [M_Latest_Month_Sale]
    VAR pms = CALCULATE([M_Total_Sales],
                        D_Calendar[Start of Month] = EDATE(td, -1))
RETURN
    DIVIDE((tms - pms), pms, 0)
```
**Purpose**: Calculates the percentage change between current month and previous month sales

**Logic**:
- `td` = Latest month date
- `tms` = Current month sales
- `pms` = Previous month sales (using EDATE to go back 1 month)
- Returns the growth percentage with zero-division handling

**Similar measures created for**:
- Profit (M_Latest_Month_Profit, M_MOM_Profit_(%))
- Shipments (M_Latest_Month_Shipments, M_MOM_Shipments_(%))
- Boxes (M_Latest_Month_Boxes, M_MOM_Boxes_(%))
- LBS_Count (M_Latest_Month_LBS, M_MOM_LBS_(%))

#### Base Measures
- `M_Total_Sales`: Sum of all sales
- `M_Total_Profit`: Sum of all profit
- `M_Total_Shipments`: Count of shipments
- Additional aggregation measures for Boxes and LBS_Count

### 📊 Insights & Findings

### Performance Highlights:
- **Dynamic filtering** enables real-time analysis across multiple dimensions
- **Salesperson performance** tracking identifies top contributors and areas for improvement
- **Product profitability** analysis reveals high-margin and low-margin items
- **Geographic distribution** shows market penetration and opportunities
- **Seasonal trends** visible through time-series analysis (Jan 2023 - Jul 2024)

### Key Analytics:
- Monitor MoM growth trends across all KPIs
- Identify shipment distribution patterns (0-50 boxes per bin)
- Track profit margins at salesperson and product levels
- Analyze LBS efficiency ratios for operational optimization
- Compare performance across order status (Cancelled, Delivered, Placed)

## 🚀 Getting Started

### Prerequisites
- Microsoft Power BI Desktop (latest version recommended)
- Access to `Choco Company Data.xlsx`

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/chocolate-sales-dashboard.git
   cd chocolate-sales-dashboard
   ```

2. **Open the Dashboard**
   - Open the `.pbix` file in Power BI Desktop
   - Ensure `Choco Company Data.xlsx` is in the correct path
   - If prompted, update the data source path

3. **Refresh Data**
   - Click "Refresh" in Power BI to load the latest data
   - Verify all visuals are displaying correctly

### Navigation Guide

**Switching Between Views:**
- Use the **custom toggle buttons** to switch between:
  - **Salesperson Performance** view
  - **Product Analytics** view

**Applying Filters:**
1. **Year**: Select 2023 or 2024
2. **Order Status**: Choose Cancelled, Delivered, or Placed
3. **Category**: Filter by Bars, Bites, or Other
4. **Countries**: Select specific country for focused analysis (see Dashboard 4)

**Viewing Different Metrics:**
- Click the **button slicer** above the line chart to toggle between:
  - Sales
  - Profit
  - Shipments
  - LBS_Count

**Exploring Geographic Data:**
- Hover over the line chart to see the **Sales by Countries** pie chart tooltip

## 📝 Future Enhancements

- Add forecasting models for sales prediction
- Include customer segmentation analysis
- Implement drill-through pages for detailed analysis
- Add competitor benchmarking
- Create mobile-optimized view
- Include year-over-year (YoY) comparisons
- Add more country-specific dashboards
- Integrate real-time data refresh
- Create automated email reports
- Add inventory management metrics

## 📸 Dashboard Screenshots

### View 1: Salesperson Performance
*Shows individual sales team performance with detailed metrics*

### View 2: Product Analytics
*Displays product-level profitability and category breakdown*

### View 3: Geographic Distribution
*Visualizes sales distribution across multiple countries*

### View 4: Filtered Country View
*Example of Australia-specific market analysis*

## 👤 Author

**Nagasai Devavarapu**
- GitHub: [@nagasai-dev](https://github.com/nagasai-dev)
- LinkedIn: [Nagasai Devavarapu](https://www.linkedin.com/in/nagasai-devavarapu)

## 🙏 Acknowledgments

- Data source: Chocolate Company Sales Database
- Built with Microsoft Power BI
- Icons from Power BI icon library