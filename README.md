![Banner](https://github.com/CARNAGE1010/AMANSHARMA.github.io/blob/main/AI_designing-with-data.gif)

# 👋 Hi, I'm AMAN SHARMA    !

### 💻 Data Analyst | SQL | Python | AWS | Power BI | Tableau | Excel

---

Welcome to my GitHub profile! I’m a passionate data analyst who loves turning data into actionable insights. With expertise in **SQL**, **Python**, and tools like **AWS**, **Power BI**, **Tableau**, and **Excel**, I enjoy building dashboards and analytical models that help businesses thrive.

![Data Science GIF](https://media.giphy.com/media/L8K62iTDkzGX6/giphy.gif) <!-- Add a relevant GIF -->

---

## 🛠 Skills & Tools

| **Category**          | **Tools/Technologies**                               |
|-----------------------|------------------------------------------------------|
| **Data Analysis**      | SQL, Excel (Advanced Formulas, Pivot Tables)         |
| **Visualization**      | Power BI, Tableau                                    |
| **Programming**        | Python (Pandas, NumPy, Matplotlib, Seaborn)          |
| **Cloud Computing**    | AWS (Data Services, EC2, S3)                         |
| **Version Control**    | Git & GitHub                                         |

---

## 🌟 Featured Projects

### 📊 [Project 1: Goods Company Sales Insights.
 <!-- Add a screenshot of your project dashboard -->
**Tools:** Power BI, SQL . 

### Data Analysis Using SQL

1. Show all customer records

    `SELECT * FROM customers;`

1. Show total number of customers

    `SELECT count(*) FROM customers;`

1. Show transactions for Chennai market (market code for chennai is Mark001

    `SELECT * FROM transactions where market_code='Mark001';`

1. Show distrinct product codes that were sold in chennai

    `SELECT distinct product_code FROM transactions where market_code='Mark001';`

1. Show transactions where currency is US dollars

    `SELECT * from transactions where currency="USD"`

1. Show transactions in 2020 join by date table

    `SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;`

1. Show total revenue in year 2020,

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";`
	
1. Show total revenue in year 2020, January Month,

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");`

1. Show total revenue in year 2020 in Chennai

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020
and transactions.market_code="Mark001";`


Data Analysis Using Power BI

1. Formula to create norm_amount column

`= Table.AddColumn(#"Filtered Rows", "norm_amount", each if [currency] = "USD" or [currency] ="USD#(cr)" then [sales_amount]*75 else [sales_amount], type any)`


---

### 📈 [Project 2: Hospitality Regional Sales Analysis.
**Tools:** Tableau, SQL, Excel 

Week-on-Week (WoW) is a type of business metric that measures changes in a specific variable 
over a period of one week compared to the previous week. It is a common way of tracking 
business performance over time and is particularly useful for analyzing trends and identifying 
areas where improvements can be made. 
Here are the metrics for which we found the WoW change% in this video: 
1. Revenue WoW change %: To get the revenue change percentage week over week. 
2. Occupancy WoW change %: To get the occupancy change percentage week over week. 
3. ADR WoW change %: To get the ADR (Average Daily rate) change percentage week over 
week. 
4. RevPAR WoW change %: To get the RevPAR (Revenue Per Available Room) change 
percentage week over week. 
5. Realisation WoW change %: To get the Realisation change percentage week over week. 
6. DSRN WoW change %: To get the DSRN (Daily Sellable Room Nights) change percentage 
week over week. 
Let’s understand WoW change% for Revenue metric as an example: 
Let’s break down this formula: 

`Var selv = IF(HASONEFILTER(dim_date[wn]), SELECTEDVALUE(dim_date[wn]),MAX(dim_date[wn])) `

This line creates a variable named selv. It checks if there is only one filter applied to the 
dim_date[wn] column. If there is only one filter, it uses the selected value of that filter; 
otherwise, it uses the maximum value of the dim_date[wn] column. 

`var revcw = CALCULATE([Revenue],dim_date[wn]= selv) `

This line creates a variable named revcw. It calculates the revenue by applying a filter on the 
dim_date[wn] column, where the value matches the one stored in the selv variable. The 
[Revenue] measure is used for this calculation. 

`Var revpw = CALCULATE([Revenue],FILTER(ALL(dim_date),dim_date[wn]= selv-1)) `

This line creates a variable named revpw. It calculates the revenue for the previous week by 
applying a filter on the dim_date[wn] column, where the value is one less than the one stored in 
the selv variable. The FILTER function combined with ALL(dim_date) ensures that the filter is 
applied to all the dates, regardless of other filters that might be active. The [Revenue] measure 
is used for this calculation. 

`DIVIDE (revcw, revpw,0)-1 `

This line calculates the percentage change in revenue WoW. It uses the DIVIDE function to divide 
the value of revcw (current week revenue) by the value of revpw (previous week revenue), with 
a specified default value of 0 in case the divisor is 0. The resulting quotient is then subtracted by 
1 to calculate the percentage change. 

The entire formula returns the week-over-week percentage change in revenue. This formula can 
be used as a calculated column or a measure in Power BI to display the WoW revenue change in 
a visual or table. 


---

### 📈 [Project 3: Adventure works bike company.
![Tableau Dashboard GIF](https://your-gif-link.com) <!-- Include a GIF of a Tableau dashboard -->
**Tools:** Tableau, SQL, Excel  
An interactive sales performance tracker built in Tableau, offering detailed insights into regional sales trends, product performance, and year-over-year growth.

---

### 📈 [Project 4: Banking Domain Data Visualization.
![Tableau Dashboard GIF](https://your-gif-link.com) <!-- Include a GIF of a Tableau dashboard -->
**Tools:** Tableau, SQL, Excel  
An interactive sales performance tracker built in Tableau, offering detailed insights into regional sales trends, product performance, and year-over-year growth.

---

## 🎯 Currently Learning

- 🧠 **Machine Learning**: Enhancing predictive modeling skills with Python.
- ☁️ **Cloud Computing**: Expanding expertise in AWS data services and infrastructure.

---

## 📊 GitHub Stats
![GitHub Stats]
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=your-username&layout=compact&theme=dark)

---

## 📫 Let’s Connect
- LinkedIn: [Your LinkedIn Profile](https://linkedin.com/in/yourprofile)
- Email: [your-email@example.com](Aman132sharma@gmail.com)

---

![Thank You GIF](https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExNHRoYmdydDZrNjh0Z2lwZHY2NnQ4cmczcjV2MHJ2NWRxd2NnZWR4cSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/SvckSy7fFviqrq8ClF/giphy.gif)
