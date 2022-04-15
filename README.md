 <p align="center">
    <img src="https://github.com/nguyenlly/math448_proj/blob/main/images/Spotify_logo.png" width="120" height="120">
     <h1 align="center">Analysis of Spotify Million Playlist Dataset Challenge</h1>
    <p align="center" class="h6">By Nguyen Ly</p>
    
## Introduction

As streaming is turning into the primary manner of interacting with music, this creates modifications to how music is consumed. This project is an evaluation of tune advice and interplay, specially on Spotify. Music advice and interplay might be tested the use of public playlists made via way of means of Spotify users. This assignment will in addition delve into the fulfillment of a song and its recognition at the streaming platform primarily based totally on playlist advice and interplay. The metrics for measuring music advice and interplay is thru the fulfillment of artist and song with recognition, playlist count, and follower count.

#### Research Questions
- What variables increase the popularity of a song?
- What is the effect of a track’s popularity on the number of Spotify playlist a track is in?
- Does having a high playlist and follower count influence an artist’s popularity, assuming that
popularity score is an indicator of interaction with an artist?

## Tools Utilized 
- Python 3
- Excel
- R

### Python Libararies
- Pandas

## Dataset Information

**Dataset Name:** Spotify Dataset 1921-2020, 600k+ Tracks | [Link to Kaggle Dataset](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks)

**Dataset Description:** Audio features of 600k+ tracks, popularity metrics of 1M+ artists

**Dataset Owner:** Yamac Eren Ay

**Source:** Spotify Web API

**Release Data of Latest Version:** April 2021

## Figures

<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure1.png" width="550" height="650"></p>
<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure2.png" width="550" height="650"></p>
<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure3.png" width="550" height="650"></p>
<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure4.png" width="550" height="650"></p>
<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure5.png" width="550" height="650"></p>
<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure6.png" width="550" height="650"></p>



## Conclusion 

- Of the 11 numerical variables examined in comparison to popularity, there is a positive linear
relationship between popularity score and six variables: playlist count, danceability, duration
in minutes, energy, loudness, and speechiness. Of those six variables, playlist count and loud-
ness have the highest value of positive correlation to popularity, with a correlation coefficient
of 0.331 and 0.345 respectively.

- A track that has a high popularity score ranging from 50 to 100, is 15 times more likely to
have a high playlist count than a track with a mid to low popularity score.
- Based on the Chi-Square Test of Independence, the p-value is statistically significant. This
meant that the p-value was less than the alpha level. Therefore, the popularity score is not
independent of playlist count.

- Having a high popularity score also mean that an artist will have a higher probability of
having a high follower count and high playlist count, assuming follower count and playlist
count are metrics for user’s interactions with an artist.

- While there is a high correlation between follower count and playlist count, there is a low
correlation between follower count and popularity score, and playlist count and popularity
score. Although these correlations are low, the correlation test reveals that the correlation
between these variables is statistically significant. This meant that the correlation between
these variables was not 0 and there is a relationship between these variables.

- Artists with a high popularity score are 10.47 times more likely to have a high playlist count
than artists with low popularity scores. The relative likelihood for an artist with a high
popularity score to have a high playlist count is 9.94 times the likelihood of an artist with a
low popularity score to have a high playlist count. Artists with a higher popularity score are
42.59 times more likely to have a high follower count than artists with a low popularity count.
The relative likelihood for an artist with a high popularity score to have a high follower count
is 4.65 times the likelihood that an artist with a low popularity score to have a high follower
count.

- Through the permutation test, we determined that the probability of having a higher playlist
count is higher for artists with high popularity scores than artists with low popularity scores,
and the probability of having a higher follower count is higher for artists with high popularity
scores than artists with low popularity scores.
