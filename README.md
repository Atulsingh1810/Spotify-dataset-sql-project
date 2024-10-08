# Spotify-dataset-sql-project

This project is structured around a database named spotify, designed in PostgreSQL. Here's a detailed description of the project's key components and objectives:

1. Database Structure
The project centers on a table called spotify, which contains a rich dataset representing information about songs, albums, and artists. The fields in the table are:

artist: The name of the artist.
track: The name of the track.
album: The album to which the track belongs.
album_type: The type of album (e.g., single or album).
danceability, energy, loudness, speechiness, acousticness, instrumentalness, liveness, valence, tempo: Various audio features that describe the track's musical properties.
duration_min: The track’s duration in minutes.
title: Another track-related title field, possibly denoting the main or featured title.
channel: The channel or platform where the track is hosted (such as a YouTube channel).
views, likes, comments: Viewer engagement metrics including views, likes, and comments.
licensed: A boolean field indicating whether the track is licensed.
official_video: A boolean indicating if there is an official music video for the track.
stream: The total number of streams for the track.
energy_liveness: A combined field possibly representing a computed or merged value of energy and liveness.
most_played_on: A categorical field representing where the track is most played (platform or channel).
2. SQL Queries
The project is divided into three levels of query complexity:

Easy Level
Tracks with more than 1 billion streams: Identifies the tracks that are extremely popular by filtering for those with over a billion streams.
List albums and their artists: Displays all albums along with their respective artists.
Total comments for licensed tracks: Sums up the number of comments on tracks that are licensed.
Tracks that are singles: Retrieves tracks that belong to albums classified as "single."
Track count by artist: Counts the number of tracks for each artist.
Medium Level
Average danceability per album: Calculates the average danceability score for tracks in each album.
Top 5 tracks with the highest energy: Lists the top 5 tracks with the highest energy scores.
Tracks with official videos: Displays all tracks that have official videos along with their views and likes.
Advanced Level (not displayed in the snippet)
Likely to include more complex queries that combine multiple fields and require aggregations, joins, or subqueries.

3. Key Insights
Focus on Track Popularity: The project emphasizes popularity metrics (streams, likes, views), allowing analysis of which songs or artists have the most significant engagement.
Track Features: It also involves analyzing musical features like danceability and energy, which are crucial for understanding the musical characteristics of popular songs.
Engagement vs. Licensing: There is a focus on the impact of licensing on audience interaction, such as views, comments, and likes.
4. Potential Applications
This database and its queries could be used to:

Analyze Music Trends: By looking at which tracks and artists perform well based on streaming and engagement data.
Understand Audience Preferences: Using features like danceability and energy to understand what makes certain tracks more popular.
Platform-Specific Insights: The most_played_on and channel fields enable insights into platform-specific performance (e.g., YouTube vs. Spotify).
This project demonstrates data-driven insights into music streaming and artist performance on a global scale
