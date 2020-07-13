# MNR-HCM datathon 2020
We introduce a new dataset that contains personal lifelog and surrounding environment data, collected periodically along predefined routes in Ho-Chi-Minh city, Vietnam. We also introduce self-developed devices as well as system architecture for gathering, storing, accessing, and visualizing data. Moreover, some exciting research topics and applications, especially for understanding correlations between people's health, air pollution, and congestion, resulting from the insights of this data set are discussed.

## Data 
### 1. Data collection
To collect data, we build the scenario as follows: Data in TP. Ho Chi Minh was collected according to the following scenario: two volunteers participated in our campaign to control motorcycles with sensors and lifelog cameras, and smartphones  were installed in the emotional tag collection application. Two volunteers drive a motorbike in the opposite direction on the predefined distance, in Table 1, at a speed of 20-30km/h. The campaign is carried out three times a day: morning, afternoon and evening during rush hour, about two hours in the approximately 17 km. We try to diversify the surrounding environment by designing the route that includes parks, traffic density, small roads, and riverside. The campaign was conducted from July 12, 2020 to July 31, 2020.
|    No.        |  Route | Feature |
| ------------- | ------------- |-----|
| 1             |Nguyen Tat Thanh - Khanh Hoi bridge - Ton Duc Thang - Nguyen Huu Canh - Nguyen Binh Khiem - Thi Nghe bridge | The main route with Riverside path, parks with many trees.    |
| 2             | Xo Viet Nghe Tinh - Dien Bien Phu - Dinh Tien Hoang - Vo Thi Sau - Cong Truong Dan Chu Roundabout  |  The main route with heavy traffic, less trees and lots of buildings   |
| 3             | Cach Mang Thang Tam - Nguyen Thi Minh Khai - Hai Ba Trung - Le Thanh Ton - Nguyen Thi Nghia  |  There are many large parks with lots of trees, crowded traffic.   |
| 4             | Nguyen Thi Nghia - Ong Lanh bridge - Hoang Dieu  | Nearby the river, traffic, less trees, lots of highrise buildings    |

          Table 1: Position and environmental features of the route for data collection

To get the feedback of volunteers safely and timely, we encourage the volunteers to stop their motorbikes whenever they meet the red traffic light or fall into the traffic congestion areas. That action can increase the correlation between air pollution, congestion, and people’s health hidden in our dataset. 

### 2. Data Description

Following are the description of data structure and direction organization.
* Image data, stored in the following folders:
   - image_tag: Contains images taken by smartphones during the different routes. Most of the images are taken at the predefined checkpoints.
   
   - photo: Contains images taken by lifelog cameras.
* Emotion tags, stored in:
   - emotion_tags: Contain information on all checkpoints of four routes in a day.

* Sensor data, stored in:
    - Sensor: The sensor value of the parameters is measuredduring the day in four routes, the parameters: urban nature, weather variables, concentration of pollutants and psycho-physiological.

* Route map: The map of four routes.
    - route_map.png 

### 3. How to download dataset?
1. Please fill out this form [Usage Agreement for the MNR-HCM Data 2020](https://drive.google.com/file/d/1gPIiz4EWDirj_zqLQ97PORfJ6yJ2piZD/view?usp=sharing)
3. Print, sign, and scan, return the form as an attachment to mnrteam19@gmail.com.
4. Our team will contact you shortly and give you link can download dataset.

### Working Notes and Overview Paper
[ICDAR '20](https://www.researchgate.net/publication/340582855_MNR-HCM_Data_A_Personal_Lifelog_and_Surrounding_Environment_Dataset_in_Ho-Chi-Minh_City_Viet_Nam)

### Citing MNR-HCM Data
If you use MNR-HCM Data in your research or wish to refer to the baseline results published in the ICDAR '20, please use the following BibTeX entry.
```
@inproceedings{10.1145/3379174.3392320,
author = {Nguyen-Tai, Tan-Loc and Nguyen, Dang-Hieu and Nguyen, Minh-Tam and Nguyen, Thanh-Duong and Dang, Thanh-Hai and Dao, Minh-Son},
title = {MNR-HCM Data: A Personal Lifelog and Surrounding Environment Dataset in Ho-Chi-Minh City, Viet Nam},
year = {2020},
isbn = {9781450375092},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3379174.3392320},
doi = {10.1145/3379174.3392320},
booktitle = {Proceedings of the 2020 on Intelligent Cross-Data Analysis and Retrieval Workshop},
pages = {21–26},
numpages = {6},
keywords = {sensors, lifelog, PM2.5, AQI, particulate matter, environment},
location = {Dublin, Ireland},
series = {ICDAR ’20}
}
```

