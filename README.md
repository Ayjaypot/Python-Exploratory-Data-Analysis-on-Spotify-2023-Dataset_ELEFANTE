# Python-Exploratory-Data-Analysis-on-Spotify-2023-Dataset_ELEFANTE
### A project that deals with the analysis of a spotify dataset that includes different questions and tasks that would test the familiarization of the different libraries in python. The dataset in question is an excel file that contains a number of columns and rows with different data types that would be explored later on.
## A. Overview of Dataset
### - How many rows and columns does the dataset contain?
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The dataset contains 953 rows and 25 columns. The code used to find it is shown below:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/5e3ada79-dc0c-4165-9893-563d23ad94c9)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The output for this code is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/b61c4a79-c812-4fdb-aace-70cb28c2990f)
### - What are the data types of each column? Are there any missing values?
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;As per the findings by using the .dtypes function from the pandas library, there are 3 data types found in the \
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dataset them being integers, objects, and float. As for missing values that are found through the use of the .isnull\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and .sum function to add find the total number of missing values as well. There were 50 missing values in the "in_shazam_charts" column\ 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and 95 missing values in the "key" column.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the data types is\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/9794e66c-b852-47d0-b9a3-7f0704593308)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the missing values is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/6a3939d2-896f-439d-a517-8b6829d8f185)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The output for data types:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/bd342b3c-6050-42b2-93df-ec9b70d7de7b)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The output for missing values:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/7c990494-9e71-4afb-8459-41baf5b6db82)

## B. Basic Descriptive Statistics
### - What are the mean, median, and standard deviation of the streams column?
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The mean, median, and mode was computed using the numpy library and the computed values are the following:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/85e35aba-65f8-4cd5-addd-97eb2135657b)\
&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the output above is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/6be83751-e16c-4588-8f31-7eec6e446387)\
&nbsp;
### - What is the distribution of released_year and artist_count? Are there any noticeable trends or outliers?
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;By using the seaborn and matplotlib libraries graphs were created for the distribution of released year and artist count.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;As for the trends, in the graph for the released year there are noticeably less tracks from the year 2000 and below and from years 2000 \
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;to 2023 there is an almost steady increases in tracks and a great increase in the years between 2010 and 2023. The graphs are shown below\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Graph for distribution of released_year:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/20a24e95-401f-404d-b661-c4e6778bc8d6)\
&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Graph for distribution of artist_count:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/5fe5f358-51f2-47e0-9e30-a54eaa0c7056)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for mean, median, mode and standard deviation is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/f0aa4465-2b54-4f1d-b3c7-99257762b8e5)\
&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the graphs is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/cf0bd8c5-9d4a-422a-8879-7301ac10bdfa)

## C. Top Performers
### - Which track has the highest number of streams? Display the top 5 most streamed tracks.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Using functions from the pandas library and the head function the top 5 tracks were found based on number of streams.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The most streamed was Blinding Lights and the top 5 are shown below:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/c9d44732-3eb0-4e16-8dec-2d2da75f070e)\
&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the output above is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/d2a0627d-4a8b-48f5-a5d4-a144e2bf2ccf)\
&nbsp;
### - Who are the top 5 most frequent artists based on the number of tracks in the dataset?
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Same as the previous question functions from the pandas library and the head function were used to find the top\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;artists based on number of tracks. The top 5 are shown below:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/e986b144-022a-4cb9-842f-89221acc9dd0)\
&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the output above is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/ac5714e5-2cde-45b3-82ed-500148b576d6)
\

## D. Temporal Trends
### - Analyze the trends in the number of tracks released over time. Plot the number of tracks released per year.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Using functions from the matplotlib and seaborn the graph for the tracks released per year was created. As for trends\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;same as earlier in the graph for the released year there are noticeably less tracks from the year 2000 and below and from\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;years 2000 to 2023 there is an almost steady increases in tracks and a great increase in the years between 2010 and 2023.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The graph is shown below:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/b6240891-262a-4cd3-bf78-900d6e1a30e0)\
&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the graph above is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/73002fbd-399e-4bbe-a262-d1c23f38bb0e)


&nbsp;
### - Does the number of tracks released per month follow any noticeable patterns? Which month sees the most releases?
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;As for number of tracks released per month, the month with the most releases is January and there is no noticeable trend except that\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;some pair of months have almost the same number of releases. The graph is shown below:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/d5d43e76-9911-413f-82e8-761d001d38f5)\
&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the Graph above is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/9ba4f9f4-f607-4baa-9f2f-f1c4f1177c8f)

## E. Genre and Music Characteristics
### - Examine the correlation between streams and musical attributes like bpm, danceability_%, and energy_%. Which attributes seem to influence streams the most?
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;As shown with the computed data almost all have a negative correlation with bpm having almost no correlation which means that none\ 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;of this attributes affect the streams much. The computed data is shown below:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/a6554f8b-008f-48f9-9223-b9bbf74c88dd)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the above data is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/671e465e-40ec-4719-81cf-63ce4175f692)\
&nbsp;
### - Is there a correlation between danceability_% and energy_%? How about valence_% and acousticness_%?
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Unlike the correlation between musical attributes and streams there is a positive correlation between danceablity and energy which\ 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;means they go up in relation to each other, while for valence and acousticness there is a negative correlation same with the streams.\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The correlation data is shown below:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/e283cd08-3a13-4443-a2eb-7ead7c8b9038)\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The code for the above data is:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/user-attachments/assets/195ed32f-20dd-4db6-a38d-51a1e447c1ba)\



## Version History
1.0 - 08/11/2024 - uploaded initial code\
1.1 - 08/11/2024 - uploaded initial code again due to error in file\
1.2 - 08/11/2024 - uploaded updated code again due to corrections in original code\





