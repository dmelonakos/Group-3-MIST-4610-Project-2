# Group-3-MIST-4610-Project-2

## Team Name and Members
Team 3

Cooper Waters [@coopw07](https://github.com/coopw07)

David Melonakos [@dmelonakos](https://github.com/dmelonakos)

Noah Hirschfield [@nbh14975](https://github.com/nbh14975)

Jacob Weiszer [@JacobWeisz](https://github.com/JacobWeisz)

Coleman Willis [@Chipolman10](https://github.com/Chipolman10)
## Dataset Description
This dataset contains information about trips over the past five years including trip distance, population staying home vs. population not staying home, the trip date, origin state code, longitude and latitude. It was obtained by the Bureau of Transportation Statistics through collecting mobile device data.

## Why this Dataset?
Lot of practical uses like figuring out which states have higher numbers of trips or higher distance of trips compared to others. The dataset also has a lot of quantitative data that we can work with to help answer questions.

## Data Applications
We can use this dataset to look at trends about which states have the highest total number of trips per capita to determine its cause and correlation to the number of people moving into the state. It can be used to identify what areas should be targeted for emissions reduction. It can also inform car manufacturers who specialize in high fuel efficiency vehicles about where they can position their stores in regions that see frequent long distance travel.

## Data Fields
![Pic 1](https://github.com/user-attachments/assets/d4f61faf-926a-447c-b91e-4926187fbe54)
![Pic 2](https://github.com/user-attachments/assets/c36da6b3-4477-4f0d-9262-5c3b799e5e7b)

## Manipulations to the Dataset
<img width="910" alt="Screenshot 2024-11-25 at 4 09 36 PM" src="https://github.com/user-attachments/assets/17255adb-c72b-47a2-a159-0547de475ddb">

We created one calculated field for our data analysis. This field finds the number of trips over 100 miles and then divides this by the county population on the average day. We took the 100-250 mile, 250-500 mile, and 500-plus mile trips and then divided them by the total population per county found in this dataset. 

## Question 1 and Why We Asked It
### Question 1


### Reasoning

## Question 1 Results and Analysis


## Question 2 and Why We Asked it
### Question 2
How has the average number of trips > 100 miles per capita daily been changing in different states over the past 5 years?
### Reasoning
We wanted to know how the percentage of people taking long distance trips was changing over time in different states and if there was a significant relationship between time and that value. If we knew which states were likely to have an increase in long distance travel, we could advertise fuel efficient vehicles in those areas, invest in real estate for lodging, invest in more efficient public long distance transportation (trains), and make any number of other investment/policy decisions.
## Question 2 Results and Analysis
### Arizona
![Gp2 azdata](https://github.com/user-attachments/assets/2fb3b06d-21e8-4ab5-85b7-a55f42cfe4e8)
R-Squared: 0.568899<br/>
P-Value:   < 0.0001<br/>
This graph shows a significant positive relationship between each consecutive month over time and the percentage of Arizona residents traveling farther that 100 miles on a daily basis. With an R-Squared of about 0.57, this means that about 57% of the variation in the percentage (y-axis values) value can be explained by the month and year (x-axis values). This ultimately means that, because there is a significant relationship between the two variables, we can expect that the percentage of Arizona residents traveling farther that 100 miles on a daily basis is likely to continue to increase, at least in the short term. 
### Georgia
![Gp2 gadata](https://github.com/user-attachments/assets/72fe5167-ba8c-4aaf-be06-301406fd9c7f)
R-Squared: 0.203504<br/>
P-Value:   0.0002975<br/>
This graph shows a significant positive relationship between each consecutive month over time and the percentage of Georgia residents traveling farther that 100 miles on a daily basis. With an R-Squared of about 0.20, this means that about 20% of the variation in the percentage (y-axis values) value can be explained by the month and year (x-axis values). This ultimately means that, because there is a significant relationship between the two variables, we can expect that the percentage of Georgia residents traveling farther that 100 miles on a daily basis is likely to continue to increase, at least in the short term, though we are less confident in this trend for Georgia than we are for Arizona. 
### New York
![gp2 nydata](https://github.com/user-attachments/assets/25512a3d-3a92-49e2-a628-de8795d410f6)
R-Squared: 0.0057639<br/>
P-Value:   0.564251<br/>
This graph shows an insignificant negative relationship between each consecutive month over time and the percentage of New York residents traveling farther that 100 miles on a daily basis. With an R-Squared of about 0.00578, we can say that about .6% of the variation in the percentage (y-axis values) value can be explained by the month and year (x-axis values). This ultimately means that, because there is an insignificant relationship between the two variables, we cannot reasonably predict any changes in the percentage of New York residents traveling farther that 100 miles on a daily basis.

### Analysis

## Conclusion
While this data set includes trips from many modes of transportation and does not decipher between them, we can infer from the results of question 1 that many are by car. When analyzing breakdown of longer trips by county, it becomes apparent that the rural counties tend to have the highest trips per capita which accounts for having to travel long distances to urban areas for work, appointments, etc. As we saw through question two, there seems to be a correlation between the states that are seeing the highest avg number of trips over 100 miles and the states with the largest growing numbers of residents and future research can help support this claim. As the U.S population grows, companies expand, and turn to more hybrid formats, more people will move to the suburbs and rural counties. It’s important for car companies to analyze where there will be high demand for fuel-efficient cars, governments to be aware of where infrastructure needs improvement, and marketers to determine what types of people are traveling out of necessity vs. for leisure. 

## Tableau Packaged Workbook
File was too large to submit through github (>25MB). We submitted the twbx in ELC.

