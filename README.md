
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

![Home](https://raw.githubusercontent.com/mukul-079/Fampay_Youtube_Assignment/master/Screenshots/1.png)



## API Endpoints
* To get all videos(GET): "http://127.0.0.1:5050/api/get_video_data/"

![Get_Video_Data](https://raw.githubusercontent.com/mukul-079/Fampay_Youtube_Assignment/master/Screenshots/2.png)
    
    

* To search from stored data(GET): "http://127.0.0.1:5050/api/search/<topic>"

![Search_Stored_Query](https://raw.githubusercontent.com/mukul-079/Fampay_Youtube_Assignment/master/Screenshots/5.png)
    

* To Insert API Key(POST): "http://127.0.0.1:5050/api/add_key"

![Insert_ADD_key](https://raw.githubusercontent.com/mukul-079/Fampay_Youtube_Assignment/master/Screenshots/6.png)
    

* To get API DB: "http://127.0.0.1:5050/api_db"

![ADD API Key DB](https://raw.githubusercontent.com/mukul-079/Fampay_Youtube_Assignment/master/Screenshots/3.png)

* To get API DB: "http://127.0.0.1:5050/video_db"

![To get Video DB](https://raw.githubusercontent.com/mukul-079/Fampay_Youtube_Assignment/master/Screenshots/4.png)


    






