# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Exploring climate data of Singapore

### Goal

My name is Amoz, I'm a GA student, taking on an interim position at as a Data Analyst at a Research Agency. The agency is pitching for Singapore Tourism Board (STB). The client has asked requested a study to find out if weather (out of the many has an effect on low visitor footfall

For this study, we're going to analyse climate trends in Singapore. Climate refers to the general weather conditions prevailing over an area for a long period. There are several aspect to studying climate that includes rainfall, temperature, relative humidity, wet build temperature, sun shine duration etc. Particular to this study, we zoom in to Rain as the main weather determinant, havwith 'total rainfall monthly' and 'number of rainy days in a month' as variable attributing to the rainfall.

That said, Singapore is ramping up up initiatives (i.e. opening newer attractions - Mandai Bird Paradise), to help the boost the tourism industry. The STB has coined Places of Interests (POIs), that includes iconic places that has entertainment, heritage and cultural value.

We then marry the two features (Rain and Visitor footfall to POI), and draw any correlations to rain as a determinant of any poor visitor footfall experienced by the POI establishments.

---

### Problem Statement

Singapore is expected to pick up with tourism in 2024. However, weather in Singapore is largely rainy, which might be a deterrence to visits in Places of Interests. This study aims to answer the question - “Does higher rainfall equate to a decrease footfall in Places of Interests?”

---

### Datasets

#### Provided Data

There are 2 datasets included in the [`data`](./data/) folder for this project. These correponds to rainfall information from 1982-2022

* [`rainfall-monthly-number-of-rain-days.csv`](./data/rainfall-monthly-number-of-rain-days.csv): Monthly number of rain days from 1982 to 2022. A day is considered to have “rained” if the total rainfall for that day is 0.2mm or more.
* [`rainfall-monthly-total.csv`](./data/rainfall-monthly-total.csv): Monthly total rain recorded in mm(millimeters) from 1982 to 2022

#### Additional Data 

The additional data included would be the Visitor Footfall experienced from the years 1990-2023. 

* [`POI_visitors`](https://tablebuilder.singstat.gov.sg/table/TS/M891071): Monthly number of visitor footfall from 1990 to 2023. The number of footfall is recorded by the '000

#### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|Date|datetime|ALL|Date is formatted in YYYY-MM format| 
|Place of Interest|object|POI_visitors|Place of Interest is limited to 16 key attractions. As long as the POIs have entertainment, heritage or cultural value| 
|Visitor Footfall|float|POI_visitors|Footfall calculated in the thousands(000). This includes any unique visitors into the Places of Interest (i.e. one person per day)|
|Rainfall in the month|float|rainfall-monthly-total|Monthly total rain recorded in mm(millimeters) from 1982 to 2022|
|No. of days rained|float|rainfall-monthly-number-of-rain-days|Monthly number of rain days from 1982 to 2022. A day is considered to have “rained” if the total rainfall for that day is 0.2mm or more|

---

#### References
* (Database) Ministry of Trade and Industry. Retrieved from https://tablebuilder.singstat.gov.sg/table/TS/M891071.   
* Lee, C. M. (Ed.). (2024, February 1). Singapore visitor arrivals up 115% to 13.6 million in 2023. CNA. Retrieved from https://www.channelnewsasia.com/singapore/singapore-tourism-increase-visitor-arrival-136-million-2023-stb-4091076. 
* Lee, L. (Ed.). (2020, August 9). Some tourist attractions finding it hard to woo locals, others unable to meet demand. Today Online. Retrieved from https://www.todayonline.com/singapore/some-tourist-attractions-struggle-woo-locals-others-unable-meet-demand. 
* Lee, Y. S. (2024, February 26). Coldplay, then taylor swift: concert economics are driving a tourism boom in singapore . CNBC. Retrieved from https://www.cnbc.com/2024/02/27/coldplay-and-taylor-swift-concerts-to-contribute-to-singapores-growth.html#:~:text=Singapore%20is%20eyeing%20%22concert%20economics,%2Drelated%20services%2C%20said%20HSBC. 
* Meteorological Service Singapore, Climate of Singapore (2021). Retrieved from http://www.weather.gov.sg/climate-climate-of-singapore/#:~:text=Its%20daily%20variation%20is%20more,during%20prolonged%20periods%20of%20rain . 
* Ng, D. (2024, January 16). A warmer singapore could spell trouble for its tourism industry, say experts. CNA. Retrieved from https://www.channelnewsasia.com/singapore/sg-tourists-climate-change-heat-sea-level-rise-warmer-weather-ecotourism-green-4050806. 
* SG101. (n.d.). Resource Constraints and Challenges. Resource Innovation. https://www.sg101.gov.sg/infrastructure/constraints-and-challenges/resinno/  
* Singapore Business Review. (n.d.). Singapore Is 4th Most Preferred Travel Destination in APAC. Retrieved from https://sbr.com.sg/hotels-tourism/news/singapore-4th-most-preferred-travel-destination-in-apac. 






