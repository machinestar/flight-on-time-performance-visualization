# Liting Data Visualization Project
## Author
By Liting
## Summary
The main goal of this project is to display the departure flight on-time performance in JFK airport (John F. Kennedy International Airport) of 2008. The on-time departure flights on each day were aggregated by week and carriers, then divided by total number of flight to calculate the percentage of departure flights which were on time. The audience will have capability to choose different carriers to display their on-time performance and make comparison. The figure will also automatically display the averaged performance and highlight the carrier with best on-time performance in each week.
## Design
#### Data Aggregation: Date or week?

The flight performance was initially plotted by dates across the whole year in my data exploration phase. However, since I would like the final visualization to show audience the performance difference between carriers, plotting multiple lines/bubbles by dates will make the whole visualzition extremely messy. So instead of dates, I used week as x axis unit to aggregate the performance for each carrier.

#### Button or Legend? 

To give audience the capability to choose from which carrier the on-time performance is displayed, I initally created buttons for each carrier. When reader click the button, the visualization will display the performance for that particular carrier. However, according to feedback of my readers, they did not like the seperate buttons, since the figure legend has already displayed each carrier name. The button introduced redundancy. They hope to simply click the legend and figure will change accordingly. I adopted their idea and used the legend as the trigger instead of buttons.

#### Single or multiple?

In the beginning, the visualization can only display one carrier performance for each week when reader click the button. This function seems not good enough according to reader. What they hope is that they can select multiple carriers to display their performance and make comparison. This change was made in final version.

#### Chart Type

The inital display will show performance for all carriers. I chose to use bubble style for individual carrier performance instead of line. Because mapping 13 lines on one single figure will make the whole visualization look messy. To show the overall performance trend over time (average line), I believe line style will do a better job in terms of illustrating the changes. 

#### Visual Encoding

The data was groupped by carriers and does not follow any particular order. So I used color hue to seperate difference categories.


## Feedback

Feedback 1: Since the legend already shows all the carrier names, why don't you just get rid of those carrier button and make the legend interactive. 

Feedback 2: Why I cannot display multiple carriers data at the same time? Displaying only one carrier at each time does not help me to understand which carrier is performing better during a specific period of time.

Feedback 3: The week number on x axis does not make sense to me. People does not know which weeks are corresponding to which month.

Feedback 4: I would like this figure to show me which carrier has the best performance.

## Resources
Interactive Legend: http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends

Mutiple Line: http://dimplejs.org/examples_viewer.html?id=lines_horizontal_stacked

Udacity Data Visualization with D3.js course: https://www.udacity.com/course/ud507

Data was downloaded from: http://stat-computing.org/dataexpo/2009/the-data.html






