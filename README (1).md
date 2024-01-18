**Forecasting Sales:**

**Understanding Weather's Role in E-Commerce**

**Project Overview**

The purpose of this project is to analyze and uncover patterns in consumer shopping habits as they relate to various factors, including weather conditions, product categories, seasonal trends, and gender differences. By investigating the correlation between online shopping behavior and these elements, our goal is to provide actionable insights to a hypothetical e-commerce startup. This will enable the company to optimize inventory and tailor paid advertising campaigns, especially in anticipation of inclement weather, to meet customer demand and enhance business operations.

**Description of Data**

Data Set 1: Online Shopping Dataset

[https://datasetsearch.research.google.com/search?src=3&query=amazon%20sales%20dataset&docid=L2cvMTF2MTVkcTU4aA%3D%3](https://datasetsearch.research.google.com/search?src=3&query=amazon%20sales%20dataset&docid=L2cvMTF2MTVkcTU4aA%3D%253)

This dataset contains survey responses with demographic data like age and gender, as well as participants' viewpoints and actions. The categorical and numerical data formats are carefully developed to help identify patterns and trends. We use this dataset to infer demographically anchored insights and correlations from respondents' answers. This method allows a deep comprehension of the surveyed population and a thorough analysis of trends and tendencies.

Data Set 2: Open Weather Map

[https://openweathermap.org/api](https://openweathermap.org/api)

The flexible OpenWeatherMap API provides real-time weather updates, detailed forecasts, and substantial historical weather data. This comprehensive service provides temperature, wind speed, and humidity data for personal and professional use. OpenWeatherMap wisely addresses user needs with several subscription rates, making weather-related projects and apps accessible. For precise and accurate weather information, the API's huge dataset and reliability are important.

Columns:

- CustomerID: A unique identifier assigned to each customer who makes a purchase.
- Gender: The gender of the customer (e.g., Male or Female).
- Location: The geographical location or city where the customer is based.
- Transaction\_ID: A unique identifier for each individual transaction or purchase.
- Product\_Description: A detailed description of the product purchased.
- Quantity: The number of units of the product purchased in the transaction.
- Avg\_Price: The average price of the product per unit.
- Delivery\_Charges: The fees charged for delivering the product.
- Coupon\_Status: Indicates whether a coupon was used, not used, or clicked for the transaction.
- Date: The date on which the transaction occurred.
- Unix Date: The Unix timestamp representing the date and time of the transaction.

Understanding weather's role in e-commerce is key for several strategic reasons, including:

- E-commerce companies can efficiently manage inventories by analyzing sales estimates. By forecasting demand trends, especially during varied weather conditions, the corporation can stock up correctly, reducing overstocking and stockouts and maximizing storage costs and product availability.

- Tailoring Marketing Strategies: Knowing how weather affects customer shopping behaviors helps marketers tailor ads. In bad weather, buyers may favor things. Recognizing these tendencies helps create promotional events and targeted ads that meet customer needs.

- Weather-related purchase patterns help e-commerce companies personalize the shopping experience. This could involve promoting weather-appropriate products, offering special promotions, or assuring swift delivery despite bad weather to boost consumer happiness and loyalty.

**Research Questions**

- How does inclement weather affect shopping habits?
- How do online shopping habits change with extreme temperatures, and is there a correlation between peak shopping periods and the most intense temperatures in a specific area?

- How does the season affect online shopping habits?

- How does gender impact online shopping habits?

- Does the severity of the weather influence online shopping behavior?

- Is there a correlation between inclement weather and product category?

**Communication Protocols**

We used Slack and Zoom sessions to constantly update each other on project progress.

**Data Tools Used**

- Cleaning Data: Pandas

- Data Visualization Tools: Pandas/NumPy/SciPy/Matplotlib/Seaborn

- Analyzing Data: Pandas / SciPy. Stats

**Results / Analysis**

To understand how weathers impact online shopping first, we imported our necessary libraries and loaded the dataset that captures consumer purchases.

![Importing libraries](https://github.com/Simian12/Project_1/blob/emely/images./Importing%20Libraries:Loaded%20dataset.png?raw=true)

After setting up our data, we clean it up by removing any parts we don't need, like extra columns that aren't useful, and making sure all the information is complete. We also change the dates into a special number that computers like to use when they talk about time. This makes it easier for us to match our sales info with weather reports from Open Weather Map later in our code.

![Clean data](https://github.com/Simian12/Project_1/blob/emely/images./clean%20dataset.png?raw=true)

In this part of the code, we focused on diversifying our data sample by randomly selecting a set number of records from each city to ensure a balanced representation. We also assigned geographical coordinates to each city, effectively 'placing' our sales data on the map. To prepare for the integration of weather information, we created new columns for weather conditions and temperatures, which are currently left blank to be populated with actual data in subsequent steps.

![Diversifying](https://github.com/Simian12/Project_1/blob/emely/images./diversifying%20our%20data.png?raw=true)

Our data sample was diversified by randomly selecting a specified amount of records from each city in this code to maintain balance. Placing our sales data on the map required assigning geographical coordinates to each city. We generated new columns for weather conditions and temperatures, which remain blank until they are filled with data.

![Random Selection](https://github.com/Simian12/Project_1/blob/emely/images./random%20sample.png?raw=true)

To avoid overusing weather data requests, we've put our improved sales data with all the new weather information into a file.

![Avoid data requests limit](https://github.com/Simian12/Project_1/blob/emely/images./avoiding%20data%20requests%20limit%20problems.png?raw=true)

This code piece examines how the weather may encourage online shopping. We use dot plots and bar charts to determine if cold or wet weather increases buying and which weather inspires the most purchases. Like we're testing if terrible weather boosts internet sales.

![Dot Plot and Bar Graph1](https://github.com/Simian12/Project_1/blob/emely/images./dot%20plot:%20bar%20chart.png?raw=true)


From the code above we got the following graphs:
![Dot Plot](https://github.com/Simian12/Project_1/blob/emely/images./dot%20plot.png?raw=true)
![Bar Graph1](https://github.com/Simian12/Project_1/blob/emely/images./bar%20chart1.png?raw=true)


We're testing if extreme temperatures affect internet shopping in this code.  We're pulling out just the information we need showing only what individuals buy, how much it costs, the temperature, and the weather.

![Tempeatures affecting internet shopping](https://github.com/Simian12/Project_1/blob/emely/images./temperature%20affecting%20online%20shopping.png?raw=true)

These three code pieces conduct comparable work but focus on distinct details. The first plot dots to show the association between weather conditions and sales quantity. The second one is doing the same but examining average item prices. The third compares sales to weather. Each plot is a mini experiment to see if weather or temperature affects internet shopping."

![Coding scatterplot1](https://github.com/Simian12/Project_1/blob/emely/images./coding%20sp1.png?raw=true) 
![Coding scatterplot2](https://github.com/Simian12/Project_1/blob/emely/images./coding%20sp2.png?raw=true)
![Coding scatterplot3](https://github.com/Simian12/Project_1/blob/emely/images./coding%20sp3.png?raw=true)

Math is used to draw a straight line through our dot charts in both instances. This line shows how temperature affects how many items are bought and how much they cost on average. Like looking for a pattern or trend. Does warmer or colder weather increase sales or prices? We can determine a link by drawing a line.

![Linear regression1](https://github.com/Simian12/Project_1/blob/emely/images./coding%20dot%20chart1.png?raw=true) 
![Linear regression2](https://github.com/Simian12/Project_1/blob/emely/images./coding%20dot%20chart2.png?raw=true)

In this code, we're sorting our sales data by season to see when people shop the most. We make a line chart to show the average sales and a bar chart to show the total sales for each season. This helps us see which season is the busiest for shopping.

![Coding salesby season](https://github.com/Simian12/Project_1/blob/emely/images./coding%20sales%20by%20season.png?raw=true)

From the code above we got the following graphs:

![bar graph1.1](https://github.com/Simian12/Project_1/blob/emely/images./bar%20graph2.png?raw=true)

![line graph](https://github.com/Simian12/Project_1/blob/emely/images./line%20graph.png?raw=true)

This code examines whether men and women shop differently. We multiply how much was bought by the price to obtain total sales, then build a bar chart to compare men and women's purchases. We also construct a histogram showing how often men and women sell specific quantities. It's like counting how much males and girls spent on shopping sprees.

![Gender coding](https://github.com/Simian12/Project_1/blob/emely/images./coding%20gender%20shopping%20behaviors.png?raw=true)

From the code above we got the following graphs:
![Bar Graph1.2](https://github.com/Simian12/Project_1/blob/emely/images./bar%20graph3.png?raw=true) 
![Histogram](https://github.com/Simian12/Project_1/blob/emely/images./histogram.png?raw=true)

In this fragment of the code, we are still trying to find out or create an algorithm to determine if weather affects buying. Our scatterplot shows the trend with a line connecting the points. This will show if consumers buy more or less in extreme heat or cold.

![scatterplot](https://github.com/Simian12/Project_1/blob/emely/images./coding%20correlation%20between%20extreme%20temps%20and%20shopping%20online.png?raw=true)

In the following codes, we're organizing our sales data by location. For each city—Chicago, California, New Jersey, New York, and Washington DC—we're making a separate list that includes only the sales from that place. This way, we can look at each city's data on its own to understand local shopping trends."

![Chicago df](https://github.com/Simian12/Project_1/blob/emely/images./dataframechicago.png?raw=true)
![California df](https://github.com/Simian12/Project_1/blob/emely/images./dataframecalifornia.png?raw=true) 
![New Jersey df](https://github.com/Simian12/Project_1/blob/emely/images./dataframenewjersey.png?raw=true)
![New York df](https://github.com/Simian12/Project_1/blob/emely/images./new%20york.png?raw=true)
![Washington DC df](https://github.com/Simian12/Project_1/blob/emely/images./washingtondc.png?raw=true)

**In the following coding fragments, we will see the coding following from its graph.**

Here we're measuring if there's a link between temperature and how much people buy in California. We calculate a number called the 'r-value' to see how strong that link is. Then we use our linear regression function to draw a line on a plot, which shows us visually whether sales go up or down with the temperature.

![California](https://github.com/Simian12/Project_1/blob/emely/images./california1.png?raw=true)

For the Chicago data, we're doing a similar analysis. We're checking if there's a relationship between how cold or hot it is and the number of products people buy. We calculate an 'r-value' to see if the relationship is strong, and then we plot this relationship to make it easy to understand at a glance.

![Chicago](https://github.com/Simian12/Project_1/blob/emely/images./Chicago1.png?raw=true)

Next, we're doing the same thing with New Jersey's data. We set up to see if the temperature is connected to how many items people are buying there. After figuring out the 'r-value' to understand this connection, we plot it to show the trend, just like we did with the other cities.

![New Jersey](https://github.com/Simian12/Project_1/blob/emely/images./Newjersey1.png?raw=true) 

And now, we look at New York. Just like before, we're checking for a trend between the temperature and shopping amounts. We calculate the 'r-value' for New York, which gives us an idea of how closely they're related, and then draw it on a graph to see the trend clearly.

![New York](https://github.com/Simian12/Project_1/blob/emely/images./newyork1.png?raw=true)

Lastly, for Washington DC, we repeat the process. We set up our variables for temperature and quantity, calculate the 'r-value' to see the strength of their relationship, and then use our linear regression function to visualize this relationship on a graph.

![Washnigton DC](https://github.com/Simian12/Project_1/blob/emely/images./washingtondc1.png?raw=true)

Here, we are creating a box plot to compare the temperature with the quantity of items purchased in California. This type of plot helps us see the range of temperatures for different amounts of items sold, giving us a visual sense of how temperature might influence shopping behavior in this region

![bp California](https://github.com/Simian12/Project_1/blob/emely/images./box%20plot1.png?raw=true)

For the Chicago dataset, we're also generating a box plot that will visualize how the quantity of items purchased may vary with different temperature ranges. This visual will help us compare and understand any trends or outliers in the purchasing behavior in relation to the local temperatures.

![bp Chicago](https://github.com/Simian12/Project_1/blob/emely/images./boxplot2.png?raw=true)

Next, we create a box plot for the New Jersey data, which will show us the spread and central tendency of temperatures when various quantities of items are purchased. This helps to visually analyze if there's a typical temperature range when people in New Jersey tend to buy more or less.

![bp New Jersey](https://github.com/Simian12/Project_1/blob/emely/images./boxplot3.png?raw=true)

For New York, a box plot is also constructed to examine how temperature influences purchase volumes. It will visually present the temperature ranges against the quantity of items purchased, helping us to discern any patterns specific to New York's shopping trends in relation to temperature.

![bp New York](https://github.com/Simian12/Project_1/blob/emely/images./boxplot4.png?raw=true)

Finally, we're looking at Washington DC during the peak shopping season. We're using a box plot to compare the quantity of items purchased with the temperature, which will show us the temperature ranges during times when people buy the most. This can highlight whether temperature swings have a noticeable impact on shopping activity in the nation's capital during busy periods.

![bp Washington DC](https://github.com/Simian12/Project_1/blob/emely/images./boxplot5.png?raw=true)

A chi-squared test is performed in this code piece to determine if weather conditions affect product categories. A chi-squared test p-value determines whether the distribution is due to chance. The p-value implies no significant relationship, hence the null hypothesis that weather conditions don't affect product category is retained.

The most often purchased category is revealed by descriptive statistics for each product category under different weather conditions.

Finally, we use a heatmap to illustrate the association between weather conditions and product categories. Color intensity indicates purchase frequency, making it easy to spot patterns and trends.

![chi-squared coding](https://github.com/Simian12/Project_1/blob/emely/images./chisquarecode.png?raw=true)

From the code above we got the following graph:

![graph 1](https://github.com/Simian12/Project_1/blob/emely/images./graph1.png?raw=true)

This code block adds a bar chart to the analysis. The seaborn counterplot tool shows product category distribution throughout weather conditions. The x-axis shows weather conditions, and the color hue shows product categories. The height of each bar shows product sales by weather conditions. Rotating the x-ticks by 90 degrees makes weather condition labels readable. This visualization helps compare product category popularity.

![sns](https://github.com/Simian12/Project_1/blob/emely/images./sns%20code.png?raw=true)

From the code above we got the following graph:

![graph 2](https://github.com/Simian12/Project_1/blob/emely/images./graph%202.png?raw=true) 

**Conclusions**

- Clear weather increases purchasing volumes, which can be used to develop marketing and sales strategies.
- Knowing that extreme weather decreases shopping activity might help firms prepare for sales downtrends and sustain consumer engagement.
- Temperature impacts regional buying patterns differently: This helps adjust marketing campaigns and promotions to various climates and seasons.
- Shopping trends vary each season. Understanding that Autumn and Winter have higher sales might help businesses stock seasonal merchandise and start suitable advertising efforts.
- Gender-specific shopping: Recognizing that women buy more often, and men buy less often but higher-value items can help segment target groups and personalize shopping.
- In bad weather, practicality drives purchases: Businesses can change their featured products to more practical ones to boost sales.

These findings can assist e-commerce platforms in better inventory management and targeted customer engagement to meet weather- and season-driven consumer needs.

**Presentation**

Our presentation can be found here [Presentation](https://docs.google.com/presentation/d/1LyQs7nkNIzMMGvZ4OeGbhQLwIT2XTHEP5LHB-bVQeiU/edit#slide=id.g2b0cddba7ba_1_75)
