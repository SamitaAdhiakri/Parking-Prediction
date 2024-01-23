This is prediction of parkign spaces of Seattle of US. LEt me say what i did for preprocessing
https://data.seattle.gov/Transportation/Paid-Parking-Occupancy-Last-30-Days-/rke9-rsvs/about_data
1. Downloaded 30days data from seattle dataset publicly available
2. there were lots of column as this one is basic one so deleted all the column irrelevent to us like Rate, area,subarea, etc
3. there are around 27 million dataset wwith 1400 parking spaces from which i selected only 1 parking spaces with SourceElementKey-1001
4. then i counted the number of rows where the occupied spaces are higher then the total space i.e. empty spaces being negative which is impossible
5. so i replaced all those rows with NaN
6. and then interpolated linearly, you can try anyway
7. now all the empty spaces are larger then 0
8. All the data are made into 5 min bins so that it will be easy for us to predict the data. 
After this data ready for prediction. if you have further question feel free to ask. I'm more than happy to answer
