# Group-3-MIST-4610-Project-2

## Team Name and Members
Team 3

Cooper Waters [@coopw07](https://github.com/coopw07)

David Melonakos [@dmelonakos](https://github.com/dmelonakos)

Noah Hirschfield [@nbh14975](https://github.com/nbh14975)

Jacob Weiszer [@JacobWeisz](https://github.com/JacobWeisz)

Coleman Willis [@Chipolman10](https://github.com/Chipolman10)
## Dataset Description
This dataset contains information about trips in the United States over the past five years including trip distance, population staying home, population not staying home, the trip date, origin state code, longitude, and latitude. It was obtained by the Bureau of Transportation Statistics through collecting mobile device data.

### Why this Dataset?
This data set has many practical uses like figuring out which states have higher percentages of trips or higher distances of trips compared to others. The dataset also has a lot of quantitative data that we can work with to help answer questions.

### Data Applications
We can use this dataset to look at trends about how different populations across the country travel (distance, frequency, growth). It can be used to identify which areas should be targeted for emissions reduction. It can also inform car manufacturers who specialize in high fuel efficiency vehicles about where they can position their stores in regions that see frequent long-distance travel.

### Data Fields
![Pic 1](https://github.com/user-attachments/assets/d4f61faf-926a-447c-b91e-4926187fbe54)
![Pic 2](https://github.com/user-attachments/assets/c36da6b3-4477-4f0d-9262-5c3b799e5e7b)

Data is collected every day and is broken down by counties (level) which are designated by the state they are within. We can assume "Population Staying at Home" and "Population Not Staying at Home" when added together equal the total population used in this dataset.

## Manipulations to the Dataset
<img width="910" alt="Screenshot 2024-11-25 at 4 09 36 PM" src="https://github.com/user-attachments/assets/17255adb-c72b-47a2-a159-0547de475ddb">

We created one calculated field for our data analysis. This field finds the number of trips over 100 miles and then divides this by the county population. We took the Trips 100-250 mile, Trips 250-500 mile, and Trips > 500 miles and then divided them by the total population per county found in this dataset. We then applied this calculation to each of the question using the average function to find the average percentage of trips greater than 100 miles taken by a given population on any given day.

## Question 1 and Why We Asked It
### Question 1
Which counties in Arizona have the most trips over 100 miles per capita on any given day?

### Reasoning
We wanted to find how the percentage of people taking long-distance trips varied between different counties in Arizona. We picked Arizona as the state to analyze for a couple of reasons, one being that it is easy to analyze from a viewer's perspective as it has a few large counties to compare. The other reason we chose Arizona is because it is one of the fastest-growing states by population in the United States, so we figured it would be interesting and practical to analyze.
## Question 1 Results and Analysis
<img width="867" alt="Screenshot 2024-11-25 at 7 27 03 PM" src="https://github.com/user-attachments/assets/d7b1aed5-b516-4401-b841-90945af799e5">

We created a heat map to display the variation of long-distance trips between counties in Arizona. The lighter shades of blue are associated with fewer trips per capita on an average day while the darker shades mean there are more long-distance trips on an average day. For example, looking at Apache County, for every 100 peope, about 9.1 long-distance trips will be taken on a given day, whereas in Maricopa County only 3.4 trips will be taken for every 100 people on a given day (detail: the dataset contained significantly more trips than total population for any given day. So, we can assume that some of these trips may be taken by the same individuals, like truckers for example). After analyzing the visualization, we noticed rural counties such as Apacha and La Paz tended to have more long-distance trips per capita while urban counties such as Maricopa (where Phoenix is) and Pima (where Tucson is) tended to have fewer long-distance trips per capita. One possible explanation for this could be because residents of the rural counties have to take a longer trip to the urban areas to get to work for the day, while the residents of the urban counties won't have to travel as far unless it is for a trip such as a vacation. One way this data could be used is for transportation companies' advertising purposes. For example, a car dealership could advertise more fuel-efficient vehicles in rural counties since their residents tend to take longer trips. State representatives can also use this data to help figure out which demographic markets they could target potential emission-reducing policies or other transportation-related policies to. Additionally, the government could use this information to improve the outreach or current standing of different methods of public transportation, such as buses and trains, into the more rural counties.

## Question 2 and Why We Asked It
### Question 2
How has the average number of trips > 100 miles per capita daily been changing in different states over the past 5 years?
### Reasoning
We wanted to know how the percentage of people taking long-distance trips was changing over time in different states and if there was a significant relationship between time and that value. If we knew which states were likely to have an increase in long-distance travel, we could advertise fuel-efficient vehicles in those areas, invest in real estate for lodging, invest in more efficient public long-distance transportation (trains), and make any number of other investments/policy decisions.
## Question 2 Results and Analysis
### Arizona
![Gp2 azdata](https://github.com/user-attachments/assets/2fb3b06d-21e8-4ab5-85b7-a55f42cfe4e8)
R-Squared: 0.568899<br/>
P-Value:   < 0.0001<br/>
This graph shows a significant positive relationship between each consecutive month over time and the percentage of Arizona residents traveling farther than 100 miles on a daily basis. With an R-Squared of about 0.57, we can say that about 57% of the variation in the percentage (y-axis values) value can be explained by the month and year (x-axis values). This ultimately means that, because there is a significant relationship between the two variables, we can expect that the percentage of Arizona residents traveling farther than 100 miles on a daily basis is likely to continue to increase, at least in the short term. 
### Georgia
![Gp2 gadata](https://github.com/user-attachments/assets/72fe5167-ba8c-4aaf-be06-301406fd9c7f)
R-Squared: 0.203504<br/>
P-Value:   0.0002975<br/>
This graph shows a significant positive relationship between each consecutive month over time and the percentage of Georgia residents traveling farther than 100 miles on a daily basis. With an R-Squared of about 0.20, we can say that about 20% of the variation in the percentage (y-axis values) value can be explained by the month and year (x-axis values). This ultimately means that, because there is a significant relationship between the two variables, we can expect that the percentage of Georgia residents traveling farther than 100 miles on a daily basis is likely to continue to increase, at least in the short term, though we are less confident in this trend for Georgia than we are for Arizona. 
### New York
![gp2 nydata](https://github.com/user-attachments/assets/25512a3d-3a92-49e2-a628-de8795d410f6)
R-Squared: 0.0057639<br/>
P-Value:   0.564251<br/>
This graph shows an insignificant negative relationship between each consecutive month over time and the percentage of New York residents traveling farther than 100 miles on a daily basis. With an R-Squared of about 0.00578, we can say that about .6% of the variation in the percentage (y-axis values) value can be explained by the month and year (x-axis values). This ultimately means that, because there is an insignificant relationship between the two variables, we cannot reasonably predict any changes in the percentage of New York residents traveling farther than 100 miles on a daily basis.

### Analysis
You can see a correlation between the population growth of a state and the average trips > 100 miles on a daily basis. Arizona (#6) and Georgia (#15) are two of the highest-growing states in the US over the last 5 years and also experienced increase in long distance travel over the past 5 years. In contrast, New York (#50) is one of the lowest-growing states and experience a slight decline in long distance travel over the past 5 years. This suggests a potential relationship between population growth and travel on a daily basis. We posit that this may be due to the liklihood that growing states are experiencing an influx of a younger population that is more predisposed to travel while declining states are being left with an older population that likes to stay closer to home. However, we would have to do more analysis to verify the accuracy of this hypothesis. Regarding the trends themselves, these observations can be useful for multiple organizations and groups of authority. For example, state governments can use this correlation to create better transportation plans based on their state's needs. For example, if we can expect long distance travel to increase over time in Arizona, we might consider investing in high-way infrastructure. This can also be helpful for automotive and travel companies, to see what areas they should target advertisements for. 

## Conclusion
While this data set includes trips from many modes of transportation and does not decipher between them, we can infer from the results of question 1 that many are by car. When analyzing the breakdown of longer trips by county, it becomes apparent that the rural counties tend to have the highest trips per capita which accounts for having to travel long distances to urban areas for work, appointments, etc. As we saw through question two, there seems to be a correlation between the states that are seeing the highest growth in average number of trips over 100 miles and the states with the largest growing numbers of residents and future research can help support this claim. As the U.S. population grows, companies expand, and turn to more hybrid formats, more people will likely move to the suburbs and rural counties. It’s important for car companies to analyze where there will be high demand for fuel-efficient cars, governments to be aware of where infrastructure needs improvement, and marketers to determine what types of people are traveling out of necessity vs. for leisure. 
## Slides
https://docs.google.com/presentation/d/1Upanl4hadiBouveNVPrEjxKoOKZ2absH1fw69a96-YI/edit?usp=sharing



## Tableau Packaged Workbook
File was too large to submit through github (>25MB). We submitted the twbx in ELC.

