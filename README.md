
# Fampay_Youtube_Assignment


### Built With
1. Python
2. Flask
3. Sqlite3
4. Docker

## Project Goal

To make an API to fetch the latest videos sorted in reverse chronological order of their publishing date-time from YouTube for a given tag/search query in a paginated response.

## Basic Requirements:

- Server should call the YouTube API continuously in background (async) with some interval (say 10 seconds) for fetching the latest videos for a predefined search query and should store the data of videos (specifically these fields - Video title, description, publishing datetime, thumbnails URLs and any other fields you require) in a database with proper indexes.
- A GET API which returns the stored video data in a paginated response sorted in descending order of published datetime.
- A basic search API to search the stored videos using their title and description.
- Dockerize the project.
- It should be scalable and optimised.

## Bonus Points Implemented

- Add support for supplying multiple API keys so that if quota is exhausted on one, it automatically uses the next available key.
- To view the stored videos with filters(with date range) and sorting options
- Optimise search api, so that it's able to search videos containing partial match for the search query in either video title or description.


## Setup for local development
- Clone the repository:
```
git clone https://github.com/mukul-079/Fampay_Youtube_Assignment.git
```

- Then install all the requirements for the project:- 
```
pip install -r requirements.txt
```
- To start the flask server
```
python app.py
```


## Home Page
* for Home page "http://127.0.0.1:5050/"

![Home](https://drive.google.com/file/d/1uB4O4mMeOxmCumEk1hXVmlkHBkFXVKAT/view?usp=share_link)



## API Endpoints
* To get all videos(GET): "http://127.0.0.1:5050/api/get_video_data/"

![Get_Video_Data](https://drive.google.com/file/d/1-6-r2YhWIpwyqfd7QKu22VzBu9MnWiWS/view?usp=share_link)
    
    

* To search from stored data(GET): "http://127.0.0.1:5050/api/search/<topic>"

![Search_Stored_Query](https://drive.google.com/file/d/1hEuK9C2DqHS0LWeouhsTOIw3PxxKXFdN/view?usp=share_link)
    

* To Insert API Key(POST): "http://127.0.0.1:5050/api/add_key"

![Insert_ADD_key](https://drive.google.com/file/d/1141pnDV4gCGFjusK8jFDz4s9G0B_zqGU/view?usp=share_link)
    

* To get API DB: "http://127.0.0.1:5050/api_db"

![ADD API Key DB](https://drive.google.com/file/d/1n461--LoyEAw9iieHqasdiN41-iX7TX9/view?usp=share_link)

* To get API DB: "http://127.0.0.1:5050/video_db"

![To get Video DB](https://drive.google.com/file/d/1yaxMMPB06yb1M7OSFa_e7VaGutiV4xPZ/view?usp=share_link)


    






