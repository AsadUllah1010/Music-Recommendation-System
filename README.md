# Music-Recommendation-System
A Music Recommendation System is an application of Data Science that aims to assist users in discovering new and relevant musical content based on their preferences and listening behaviour. 
# Introduction
Music Recommendation Systems operate through intricate algorithms that analyze vast amounts of data about users’ musical interactions, such as their listening history, liked tracks, skipped songs, and even explicit user preferences conveyed through ratings or feedback. These data points are instrumental in constructing comprehensive user profiles, delineating individual tastes and preferences. In the initial phase, the system employs various data preprocessing techniques to cleanse and organize the information efficiently. Subsequently, the system uses recommendation algorithms, such as collaborative filtering, content-based filtering, and hybrid approaches, to generate music recommendations. As users continually interact with the system, it accumulates additional data, refining and updating their profiles in real time. Consequently, the recommendations become increasingly precise and aligned with the user’s evolving musical preferences. The Spotify API is a set of rules and protocols provided by Spotify developers. It enables developers to interact with Spotify’s vast music catalogue and collect music-related data. Through the Spotify API, developers can access information such as tracks, albums, artists, playlists, user profiles, and play history, among other features, empowering them to build innovative applications and services that integrate seamlessly with the Spotify platform. To build a Music Recommendation System using the Spotify API, we are required to collect real-time music data from Spotify. For this task, we need a Spotify developer account to get our credentials from Spotify to access their data. Below is the process you can follow to sign up for the Spotify developer account and get your credentials:
<br>
<br>
Step 1: Create a Spotify Account
<br>
For a Spotify developer account, you need an account at Spotify. If you don’t use Spotify, create an account. You don’t need to purchase any subscription to get your credentials. Once you have created an account at Spotify (or you already have one) log in to your account from your web browser.
<br>
<br>
Step 2: Go to Your Spotify Developer Dashboard
<br>
Once you have created an account at Spotify, you need to log in to your Spotify developer dashboard. Here’s the link to the dashboard. As you will be using this developer account for the first time, sign the agreement and verify your email. After these steps, we can move to the next step.
<br>
<br>
Step 3: Create An App
<br>
Once you have verified an email, you will see an option to create an app in your dashboard, as shown in the image below. Click “Create app” and move to the next step.
<br>
<br>
Step 4: App Description
<br>
Fill in the app description. 
<br>
<br>
Step 5: Copy Your Client ID and Client Secret
<br>
After filling in the app description, you will be redirected to your id and password. If you click “View client secret”, you will see your password. Copy your credentials so that you can use them while building a Music Recommendation System using Python.
<br>
<br>
I hope you have understood what a Music Recommendation System is. Now, in this section, I’ll take you through building a Music Recommendation System using Spotify API and Python. To get started with building a Music Recommendation System, we first need to have an access token. The access token serves as a temporary authorization credential, allowing the code to make authenticated requests to the Spotify API on behalf of the application. 

# Feature
Spotify API

# Conclsusion
we used a playlist ID: “37i9dQZF1DX76Wlfdnj7AP”. The code then calls the get_trending_playlist_data function to extract music data from the specified playlist using the provided access_token. The collected music data is stored in a DataFrame named music_df. Finally, the code prints the DataFrame to display the extracted music data. You can also add your playlist id here. If your playlist link is (https://open.spotify.com/playlist/37i9dQZF1DX76Wlfdnj7AP), the playlist ID is “37i9dQZF1DX76Wlfdnj7AP”, which is what you would replace with my playlist id within the above code snippet. The above function takes the release date of a music track as input, which is provided in the format ‘YYYY-MM-DD’. It then uses the datetime.strptime function from the Python datetime module to convert the release date string to a datetime object. This conversion allows us to perform arithmetic operations with dates. The function then calculates the time span between the release date of the track and the current date (today’s date) using datetime.now() – release_date. This results in a timedelta object representing the time difference between the two dates. The weighted popularity score is computed based on the time span. The formula to calculate the weight is 1 / (time_span.days + 1). The time_span.days attribute of the timedelta object gives the number of days in the time span between the release date and today. Adding 1 to the number of days ensures that the weight is never zero, even for very recent releases, as this would lead to a division by zero error. The idea behind this formula is that the weight decreases as the time span between the release date and today increases. More recent releases will have a higher weight, while older releases will have a lower weight. As a result, when combining this weighted popularity score with other factors in a recommendation system, recent tracks will have a more significant impact on the final recommendations, reflecting users’ potential interest in newer music.
<br>
<br>
So, I hope you liked this article on building a Music Recommendation System using the Spotify API and Python. A Music Recommendation System is an application of Data Science that aims to assist users in discovering new and relevant musical content based on their preferences and listening behaviour.

# Contributing
If you are interested in contributing to the project, please create a fork of the repository and submit a pull request. All contributions are welcome and appreciated.
