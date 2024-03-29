# COVID-19 impact on used cars market in Serbia

### Data source: [polovniautomobili.com](http://polovniautomobili.com)

#### Data parameters:
 - Marka - Brand of the car
 - Model - Model of the car
 - Godiste - Year of production
 - Kilometraza - Mileage
 - Karoserija - Car type
 - Gorivo - Fuel type
 - Kubikaza - Engine volume
 - Snaga - Engine power (BHS)
 - Cena - Car price in euros
 - Godina - Year of getting the data

Parameter "Godina" shows when the data was scraped from site polovniautomobili.com 

With this analysis I'm trying to understand the impact that COVID-19 had on used cars market in Serbia through examining the same (almost the same) dataset but just two years apart, from 2019. and one from 2021. The web-scraping technique was the same in both cases - scrape first two pages of car ads (with specifications) for each model and save it to csv file, more on this here: [webScraper](https://github.com/trsavi/Polovni-Automobili-Webscraper). With this sort of data gathering, there shouldn't be more than 60 cars per model per year, so total of max 120 different cars per car model. 

#### Check the [Jupyter Notebook](https://github.com/trsavi/Covid19-impact_on_usedCars_in_Serbia/blob/main/Analysis%20and%20Visualization.ipynb)

**Important info for those who do not want to review in detail what I did in Jupyter Notebook**
 * **Max car price was limited to 30.000 euros**
 * **Car mileage was limited between 20.000 - 400.000 km**
 * **Year of production was limited to greater than 1995.**
 * **Engine power was limited to 350 BHP.**
 * **Min cars per model per year of collecting the data >25 cars -> at least 50 cars per model for both years (2019, 2021)**

*Keep this in mind because every variation in these factors could result in different results in the end.*

### Dashboard created in Tableau 

![Dashboard 1](https://user-images.githubusercontent.com/26121130/139915809-89f5c9f5-f843-4315-94f7-4c244f31ada7.png)


## Conclusion

Based on this data, there was an average price increase. Overall, price increase was 6.85% but in the last decade (on cars that are not older than 10 years from both 2019 and 2021) the price increase was around 15%. The biggest difference was with petrol fueled cars (around 20%) and with limousine type vehicles (around 5%). With French manufacturers (Peugeot, Citroen, Renault), apart from the "Other" manufacturers (Ford, Volvo, Seat), the price difference was highest (around 8%) while car manufactured (originally) in Italy was lowest (going into negative -1% decrease in price). When it comes down to car brands, the biggest price difference was with Nissan cars (around 15%) and the least with Kia cars. 


**Note**: *This dataset and analysis is not sufficient to represent general trend of price increase during the first two years of COVID-19 impact. The analysis should accelerate further research on this topic with more data.*

