# Spotify Music Analysis: Most Streamed Songs of 2023

### Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Landing Page and Methodology](#landing-page-and-methodology)
- [Data Source](#data-source)
- [Tools and Techniques Used](#tools-and-techniques-used)
- [Type of Analysis Used](#type-of-analysis-used)
- [Key Performance Indicators](#key-performance-indicators)
- [Data Analysis and Results](#data-analysis-and-results)
- [Recommendations](#recommendations)

### Project Overview
This project explores Spotify’s most-streamed tracks in 2023. Using Power BI, I created a visually engaging dashboard to analyze key metrics such as total streams, top-performing artists, and audio features like energy, danceability, and mode (Major/Minor).
The goal was to transform raw music data into meaningful insights using Power Query, DAX, and strong visual storytelling.
![Spotify Music Analysis Dashboard Screenshot](https://github.com/user-attachments/assets/128578a6-18af-4b2b-a48c-0a301a03f353)


### Objectives
- Analyze top artists and tracks by global stream count
- Understand how track features (energy, valence, etc.) relate to popularity
- Create an intuitive, Spotify-themed dashboard
- Build a foundation for interactive exploration (Part 2)

### Landing Page and Methodology
| Column Name        | Description                                                                  |
|--------------------|------------------------------------------------------------------------------|
| track_name         | Title of the song                                                            |
| artist(s)_name     | Name of the artist(s)                                                        |
| streams            | Total number of Spotify streams                                              |
| release_date       | Date the song was released (merged from day, month, year)                   |
| danceability       | A measure (0–100) of how suitable a track is for dancing                    |
| energy             | Intensity and activity level of the track (0–100)                           |
| valence            | Positivity of the musical content (0–100)                                   |
| mode               | Key mode: 1 = Major, 0 = Minor                                               |
| instrumentalness   | Probability that the track is instrumental (0–100)                          |

### Data Source
You can download the dataset used for this project [here](https://docs.google.com/spreadsheets/d/11eiH_HurRXnbymNc4pskPdKhnCtC79Tg/edit?gid=1562142739#gid=1562142739).

### Tools and Techniques Used
- Power BI (for dashboarding and visuals)
- Power Query (for data transformation)
- DAX (for calculated measures and KPIs)
- Basic Data Cleaning & Transformation Techniques

### Type of Analysis Used
The analysis conducted in this project is Exploratory Data Analysis (EDA). The main purpose of EDA is to examine datasets, summarize their key characteristics, and uncover patterns or anomalies using both visual and quantitative methods. Here's how it was applied:

1. Descriptive Statistics
- Aggregated basic metrics such as the total number of streams, tracks, and artists
- Calculated averages to understand central tendencies (e.g., average streams per track)

2. Feature Analysis
- Analyzed numerical audio features such as danceability, energy, valence, etc., to understand how musical attributes relate to performance
- Converted values to percentages or normalized scales where needed (0–100 scale)

3. Categorical Distribution
- Evaluated how different categories (e.g., Mode: Major vs. Minor) influence streaming behavior
- Used a donut chart to visualize the proportion of modes

4. Time-Based Analysis
- Merged multiple columns to form a unified release_date
- Used a line chart to observe how stream volume changed over time, revealing trends in release strategies

### Key Performance Indicators
- Total Streams
- Total Tracks
- Average Streams
- Total Artists
- Top 10 Artists by Stream Count
- Most Streamed Track with Feature Breakdown
- Mode Distribution (Major/Minor)

### Data Analysis and Results
The dashboard features several visuals and DAX measures designed to answer core business questions and highlight streaming trends:

1. KPIs (Card Visuals)
- Total Streams: 489 billion
- Tracks: 952
- Average Streams: 514 million
- Total Artists: 644

These values provide a quick, high-level view of the dataset.

2. Top 10 Artists by Total Streams (Bar Chart)
- Ranked artists such as The Weeknd, Taylor Swift, and Ed Sheeran
- Helped identify which artists dominated the streaming space in 2023

3. Most Streamed Track (Image + Properties)
- Highlighted Blinding Lights as the #1 track
- Provided feature breakdowns like Energy: 80, Danceability: 50, Valence: 60

4. Distribution by Musical Mode (Donut Chart)
- Showed 57.7% of the tracks are in Major mode and 42.3% in Minor
- Suggested a listener preference toward brighter/more uplifting tracks

5. Streams by Release Date (Line Chart)
- Displayed a clear surge in popular track releases post-2010
- Suggested a shift in listening habits and digital streaming growth

6. Top 5 Most Streamed Tracks (Image Tiles)
- Gave visual emphasis to standout hits, combining data and artist recognition

Each of these visuals ties back to a core question like:
- Who are the top-performing artists?
- What musical qualities define popular tracks?
- How have streaming behaviors evolved?

### Key Insights
1. Highly Streamed Tracks Tend to Be Upbeat and Positive
- The top-streamed tracks, such as Blinding Lights and Shape of You, score high in valence (positivity) and danceability, suggesting that listeners gravitate toward emotionally uplifting and rhythm-friendly music.
- These tracks also fall mostly in the Major key, supporting the trend toward happy-sounding songs.

2. A Few Artists Dominate the Streaming Landscape
- Out of 644 unique artists, the top 10 alone account for a large share of total streams.
- Artists like The Weeknd, Taylor Swift, and Ed Sheeran lead the chart, indicating a winner-takes-most dynamic in music streaming.

3. Modern Tracks Outperform Older Releases
- A time-series analysis of release dates versus streams reveals a sharp increase in streaming volume for tracks released after 2015, with a significant surge post-2020.
- This trend aligns with the growth of streaming platforms and shifting consumer behavior toward digital-first music consumption.

4. Most Tracks Are in Major key
- Approximately 58% of tracks are in Major mode, which typically evokes happier and brighter emotional tones, compared to Minor mode.
- This implies that streaming audiences may favor songs that are more emotionally positive.

5. Track Properties Can Guide Playlist Design
- Key musical features like Energy, Danceability, and Valence vary across tracks and can be used to segment songs into playlists (e.g., “Chill Vibes”, “Workout”, “Party Hits”).
- The visualization of these properties helps understand what elements make a song “popular.”

6. Instrumental Tracks Are Rare
- Most of the streamed tracks have very low instrumentalness scores, reinforcing the popularity of vocal-driven songs over purely instrumental ones.

### Recommendations
Based on the insights drawn from the Spotify streaming data, here are several recommendations that could help both artists and platform stakeholders make more informed decisions:

1. Music Producers & Artists: Optimize Musical Features
- Danceability & Valence:

The most streamed tracks typically exhibit moderate danceability and high valence, indicating that upbeat and emotionally positive songs tend to perform better. Artists should aim to compose tracks that resonate emotionally with listeners while remaining rhythmically engaging.
- Energy Levels:

Tracks with moderate to high energy scored higher on stream counts, suggesting a preference for vibrant, active songs that energize listeners.
- Recommendation: Artists can use tools like Spotify’s audio feature analysis or third-party DAWs to fine-tune these values during production.

2. Spotify Marketing & Curation Teams: Strategic Promotion
- Top Artist Dominance:

A small number of artists like The Weeknd, Ed Sheeran, and Taylor Swift accounted for a large share of total streams. This suggests a potential to:
    - Promote emerging artists to diversify listening behavior
    - Create playlists that balance chart-toppers with new talents

- Recommendation: Use this data to tailor curated playlists and campaigns based on high-performing artist clusters and track features.

 3. Release Strategy: Focus on Recent Years
- The stream trend line shows a clear spike in post-2010 releases, especially between 2019 and 2023. This may correlate with streaming platform maturity and user growth.
- Recommendation: New artists should prioritize digital-first strategies. Legacy labels can consider re-releasing or promoting older tracks with modern edits to capture today's streaming audience.

4. Playlist Curation Based on Mood
- The strong presence of Major mode (57.7%) indicates a preference for uplifting and emotionally positive music.
- Recommendation: Spotify and similar platforms could develop mood-specific playlist categories such as:

   - Feel-Good Energy (High Valence + High Danceability)

   - Chill Evenings (Low Energy + Minor Mode)

This data-driven approach to playlist segmentation could lead to higher engagement and user retention.






