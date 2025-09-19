| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Critique & Design

## Step one: the visualization
I selected this data visualization from MakeOverMonday. The Original link is: https://resume.io/blog/which-country-gets-the-most-paid-vacation-days
<img width="2400" height="2614" alt="image" src="https://github.com/user-attachments/assets/4f2cca00-9faf-4926-b86a-56c294e14938" />

I chose it because the topic is very interesting, and is closely related to our lives. I was immediately attracted by the design. It is engaging and vivid, with clear strengths such as using a world map to directly show paid vacation days across countries. At the same time, it has some obvious weaknesses. For example, too many lines distract the viewer and make the chart look cluttered. Besides, since it contains a large amount of data, there is plenty of room for adjustment and improvement.

## Step two: the critique
Data Visualization Effectiveness Profile

## Step three: Sketch a solution
![d095f71d7f0401b6b22b42dc26bcfa1](https://github.com/user-attachments/assets/d5aba0c2-e232-4afb-8435-2373b2263333)

I think the original visualization provides a broad, general understanding of the number of paid vacation days worldwide. However, I want my redesigned chart to be more intuitive for job seekers, job hoppers, or immigrants who may consider paid vacation days as an important factor in their career decisions.

Therefore, I plan to use a bar chart, sorted in descending order by the number of paid vacation days. I will calculate the global average of paid vacation days and use it as a benchmark: countries above the average will be highlighted in blue, while those below the average will be highlighted in yellow. The color would be gradient to indicate the relative number of days within each group. This way, the audience can easily observe the global distribution of paid vacation days and make comparisons with their own country.

## Step four: Test the solution

During class, I received critiques from my peers on my sketch.

Since my sketch did not include any textual information, I had to verbally explain the meaning of the chart. This increased the difficulty for everyone to immediately understand both the visualization and the data. And we have walk through some problems together:
1. The current arrangement made it difficult to clearly see comparisons or differences at first glance.
2. The large amount of data placed in the chart made it hard to quickly extract useful insights.
3. Several people pointed out that categorizing the data by region would make the visualization easier to read and more meaningful as we can compared different region.
4. The biggest debate was about the value of this visualization. Some believed the data simply aimed to show the number of paid vacation days across countries, which was enough. Others argued that only showing paid vacation days was not useful and that additional contextual data should be introduced. And this led to another discussion: if more data should be added, what kind of data would make the visualization more meaningful?

After the discussion, I decided to make the following changes for my final visualization:
1. Create a story-driven and engaging title so that readers can quickly understand the purpose and meaning of the chart.
2. Group the data by region and keep only a selected portion of the data. By reducing the amount of data shown, the visualization will become clearer and easier to read.
3. Introduce an additional dataset that connects meaningfully with paid vacation days, so that the visualization is not only descriptive but also more useful for interpretation and decision-making.
   
## Step five: build the solution
<div class='tableauPlaceholder' id='viz1758252373808' style='position: relative'><noscript><a href='#'><img alt='Who Works Less but Earns More?Paid Vacation Days vs. GDP in the U.S. compared to Europe ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Wh&#47;WhoWorksLessbutEarnsMorePaidVacationDaysvs_GDPintheU_S_comparedtoEurope&#47;final&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='WhoWorksLessbutEarnsMorePaidVacationDaysvs_GDPintheU_S_comparedtoEurope&#47;final' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Wh&#47;WhoWorksLessbutEarnsMorePaidVacationDaysvs_GDPintheU_S_comparedtoEurope&#47;final&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1758252373808');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                      
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

**Process Documentation**
1.Initial decision
Based on the feedback, I first categorized the data by region. Since Europe has a reasonable number of countries, and European countries vary in their level of development and represent different patterns, I chose to keep only European countries. Then, from my perspective as someone currently in the United States, I decided to use the U.S. as a baseline and compare it against Europe.

2.Adding contextual data
To make the visualization more meaningful, I introduced another dataset: GDP per capita (current US$) from World Bank data. This allowed me to connect economic development with paid vacation days, making the chart more insightful.

3.Data preparation
a. I edited the dataset in Excel, keeping only the European countries and the U.S.
b. I retrieved GDP per capita data for these countries from the World Bank and added it into my Excel sheet.
c. I further divided European countries into four regions: Eastern, Southern, Western, and Northern Europe.

4.First attempt in Tableau: scatterplot
My first trial was a scatterplot, with GDP per capita on the x-axis and total paid vacation days on the y-axis. While it clearly showed the difference between the U.S. and Europe, there were some issues:
a. Some data points were too close, making it hard to distinguish individual countries.
b. The chart looked sparse and empty overall.
c. Internal comparisons within Europe were difficult to interpret.
<img width="1024" height="1080" alt="image" src="https://github.com/user-attachments/assets/d418815a-9d6c-405f-a682-0bd7ae2c28a7" />

5.Second attempt: bar chart
I then tried a bar chart with countries on the x-axis and paid vacation days on the y-axis, sorted by GDP. I used color to distinguish regions. However, the chart became too cluttered and difficult to read, so I abandoned this option.

6.Final method: Dual Axis chart
I found a workable solution with a dual axis design:
a. The first axis: a bar chart with countries on the x-axis and paid vacation days on the y-axis, sorted in descending order by paid vacation days.
b. The second axis: a line chart with countries on the x-axis and GDP on the y-axis, aligned with the same order as the bar chart.
c. Overlaid the two charts to create a combined visualization.
d. Highlighting comparisons: To emphasize the comparison between the U.S. and European countries, I added a reference line for U.S. GDP. This makes it easy to quickly identify which countries have a GDP per capita higher than the U.S., while simultaneously comparing vacation days.

## References
Watson, Bethany. “Which Country Gets the Most Paid Vacation Days?” Resume.Io, November 14, 2022. https://resume.io/blog/which-country-gets-the-most-paid-vacation-days.

World Bank Open Data. “World Bank Open Data.” Accessed September 19, 2025. https://data.worldbank.org.

## AI acknowledgements
I used ChatGPT to brainstorm what additional variables could make the visualization more meaningful. I proposed “Average monthly income” and similar economic indicators; ChatGPT recommended using GDP per capita (current US$) for clearer cross-country comparability and pointed me to the World Bank for datas

Chatgpt was used to guide me in using Tableau, providing me with detailed step-by-step instructions to help me achieve the operations I wanted in Tableau.
