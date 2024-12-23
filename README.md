# GenreWise YouTube Scraper 

## Overview
This application is designed to generate a list of the top 500 music videos from YouTube, collecting detailed information about each video and saving it in a CSV file. The genre (in this case, music) is dynamically inputted by the user, allowing the script to fetch videos in real-time for the music genre without manual intervention.


## Features
The application allows for dynamic genre input, where the user can specify the genre as music to fetch top music-related videos. This input is flexible and allows the script to regenerate data for the music genre on demand, making the process efficient and adaptable.

## How the YouTube Scraper Works
1. API Key Setup:

> To interact with the YouTube Data API v3, you first need to create a project in Google Cloud Console and enable the YouTube Data API v3 for that project.

> After enabling the API, you generate an API key. This key is required for making authorized requests to the API and retrieving data from YouTube.
2. User Input (Genre):

> The user inputs the genre they want to fetch data for (e.g., music).
The genre is used to query YouTube’s data and fetch the top 500 videos for that genre.

3. Making API Requests:

> The script sends requests to the YouTube Data API v3 using the provided API key. It specifically queries the YouTube API’s search endpoint to retrieve videos based on the genre (in this case, music).

> Fetching Data for Each Video: The script fetches data for each video in the top 500 list. For each video, it retrieves detailed information such as Video URL, Title, Description, Channel Title, Tags, View Count, Comment Count, Video Duration, Captions Availability.


For videos with captions available, the script uses the API to download captions and saves them in the CSV file. This may involve additional requests to the YouTube API to fetch the captions' text.
