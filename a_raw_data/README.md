# Raw data

Three sets of data is downloaded from LTA datamall through monthly updated API:

1. origin_destination_bus_YYYYMM.zip: these are the files recording the bus OD ridership in weekdays and weekends, 
2. origin_destination_train_YYYYMM.zip: the files recording the train OD ridership in weekdays and weekends, 
3. transport_node_bus_YYYYMM.zip: these files record the bus stop based number of tap-in and tap-out passengers. 



The YYYYMM for this study include: 201911, 201912, and 202001. 



Because the LTA team had informed us that the bus OD data prior to 2020 March had some duplication issue, so it is needed to add some data-preprocessing to scale down the flows. The transport_node_bus dataset (tap-in/tap-out) are used to perform the scale-down processing. 



For the detail of data source: https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html

The API guide: https://www.mytransport.sg/content/dam/datamall/datasets/LTA_DataMall_API_User_Guide.pdf

- section 2.6 PASSENGER VOLUMEBY ORIGIN DESTINATION BUS STOPS for **bus OD**
- section 2.7 PASSENGER VOLUME BY ORIGIN DESTINATION TRAIN STATIONS for **train OD**
- section 2.5 PASSENGER VOLUME BY BUS STOPS for **bus stop tap-in-and-out**



[API Terms of service](https://www.mytransport.sg/content/mytransport/home/dataMall/api-terms-of-service.html) and [Singapore Open Data Licence](https://www.mytransport.sg/content/mytransport/home/dataMall/SingaporeOpenDataLicence.html)

 