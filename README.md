# Bank Marketing Funnel Analysis

This project analyzes a bank marketing campaign dataset to help a business understand lead quality, funnel drop-off, conversion behavior, and optimization opportunities.

## Project Goal

The goal is to answer four key business questions:

1. Where are users dropping off in the funnel?
2. Which channels bring high-quality leads?
3. How can conversion rates be improved?
4. Which stages need optimization?

## Dataset

The analysis uses the `bank-full.csv` dataset, which contains customer and campaign information from a bank direct marketing campaign.

Important columns used in the analysis:

- `y`: Whether the customer subscribed to the term deposit
- `contact`: Contact channel used for the customer
- `campaign`: Number of contacts performed during the campaign
- `duration`: Duration of the last contact in seconds
- `poutcome`: Outcome of the previous marketing campaign
- `housing`: Whether the customer has a housing loan

## Tools and Libraries

This project uses:

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Analysis Performed

### 1. Funnel Drop-off Analysis

The campaign contact count is converted into funnel stages:

- 1st contact
- 2nd contact
- 3rd contact
- 4-5 contacts
- 6+ contacts

The notebook calculates conversion rate at each stage to identify where users are dropping off.

### 2. Channel Quality Analysis

The `contact` column is used to compare lead quality across channels such as:

- Cellular
- Telephone
- Unknown

Each channel is evaluated using total leads, conversions, conversion rate, average call duration, and average number of contacts.

### 3. Conversion Improvement Analysis

Customer segments are created using:

- Contact channel
- Previous campaign outcome
- Housing loan status

The highest-converting segments are identified so the business can prioritize better leads.

### 4. Stage Optimization Analysis

The notebook combines funnel stage and call duration buckets to identify low-performing areas with enough lead volume to optimize.

Call duration buckets include:

- Under 1 minute
- 1-3 minutes
- 3-5 minutes
- 5-10 minutes
- 10+ minutes

## Key Business Insights

The analysis helps identify:

- Contact stages where conversion rates decrease
- Channels that generate better-quality leads
- Customer segments with stronger conversion potential
- Low-converting stages that need process improvement

## How to Run

1. Open `Task3.ipynb` in Jupyter Notebook or VS Code.
2. Make sure the dataset `bank-full.csv` is in the project folder.
3. Install the required libraries if needed:

```bash
pip install pandas matplotlib seaborn
```

4. Run the notebook cells from top to bottom.

## Project Files

```text
Task3.ipynb      Main notebook containing the analysis
bank-full.csv    Full bank marketing dataset
bank.csv         Smaller version of the dataset
bank-names.txt   Dataset description
README.md        Project documentation
```

## Expected Output

The notebook produces:

- Summary tables for each business question
- Conversion rate calculations
- Funnel drop-off visualization
- Channel quality chart
- Segment performance chart
- Funnel stage and duration heatmap

## Conclusion

This project provides a practical business view of campaign performance. It can help marketing teams prioritize high-quality leads, improve weak funnel stages, and focus resources on the channels and customer segments most likely to convert.
