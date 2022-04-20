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

## Dataset Information

### Spotify Million Playlist Dataset Challenge

**Dataset Name:** Spotify Million Playlist Dataset Challenge | [Link to Dataset](https://www.aicrowd.com/challenges/spotify-million-playlist-dataset-challenge#dataset)

**Dataset Description:** The dataset contains 1,000,000 playlists, including playlist titles and track titles, created by users on the Spotify platform between January 2010 and October 2017.

**Dataset Owner:** Spotify

**Source:** Spotify

**Release Data of Latest Version:** September 2020

<hr>

### Spotify Dataset 1921-2020, 600k+ Tracks

**Dataset Name:** Spotify Dataset 1921-2020, 600k+ Tracks | [Link to Kaggle Dataset](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks)

**Dataset Description:** Audio features of 600k+ tracks, popularity metrics of 1M+ artists

**Dataset Owner:** Yamac Eren Ay

**Source:** Spotify Web API

**Release Data of Latest Version:** April 2021



## Figures

<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure1.png" width="650" height="450"></p>
<p align="center">Histogram showing distribution of popularity score of tracks in the Spotify Million Playlist
Dataset. The two red lines indicate quartile 1 and quartile 3 respectively</p>

### Findings

The distribution of the histogram is normal and unimodal,
with a mode at 40 points. It has a minimum value of 0 points and a maximum value of 90 points.
The first quartile is at 29 points. The third quartile is at 49 points. The median and mean are 39
and 38.92986 respectively

<hr>

<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure2.png" width="650" height="450"></p>
<p align="center">Scatterplots of popularity scores vs 11 numerical variables. The blue line represents the
generalized additive model and the red line represents the linear model.</p>

### Findings 

From the figure, there is a positive linear relationship between popularity and 6 numerical variables.
These are count, danceability, duration_min, energy, loudness, and speechiness. While some of
these variables are not well modeled to a linear model, this positive linear relationship suggests
that as these variables increases, popularity also increases.

<hr>

<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure3.png" width="650" height="450"></p>
<p align="center">Distribution of popularity scores in dataset</p>

### Findings
Values between Q3 and Q1 will be categorized as mid, and values above Q3
will be categorized as a high or high outlier. For popularity scores, a low score is between 0 and 28
points. A medium score is between 29 to 49 points, and a high score is between 50 to 79 points. The
outliers will be kept and will have their level which is between 80 and 100 points. As for playlist
counts, a low playlist count is between 1 and 2 playlists. A medium playlist count is between 3 to
37 playlists, and a high playlist count is between 37 to 46574 playlists.
<hr>

<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure4.png" width="650" height="450"></p>
<p align="center">Figure of scatterplot with linear regression and correlation of playlist count, followers
count, and popularity score.</p>

### Findings

There is a strong linear relationship between playlist
count and follower count, the graph of playlist count and the graph of popularity score and follower
count and popularity score does not have a strong linear relationship. This relationship can be
seen with the correlation coefficient between playlist count and follower count of 0.70, which is
a strong correlation. However, the correlation coefficient for playlist count and popularity score
and the correlation for follower count and popularity score is 0.19 and 0.23 respectively, which is
a low to moderate correlation.

<hr>

<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure5.png" width="650" height="450"></p>
<p align="center">Histogram of differences in mean-difference in playlist count and popularity score of an
arist.</p>

### Findings

While lines were added to show the difference in means of the dataset (which were at 1272.685 and
1272.685)onto the resampling from the permutation test, the lines were outside the distribution of the permutation test. The p-value for this test is 2e − 04 meaning that the p-value is statistically significant.
<hr>

<p align="center"><img src="https://github.com/nguyenlly/math448_proj/blob/main/images/figure6.png" width="650" height="450"></p>
<p align="center">Histogram of differences in mean-difference in follower count and popularity score of an
arist.</p>

### Findings
The differences in
mean-difference of follower count can be seen in Figure 5, where the resampling of differences in
mean-difference have a distribution between -10,000 and 15,000. However, the difference in mean-difference for the dataset is at -204527.6 and 204527.6 which is not included within the resamplingrange. The p-value for this permutation test is at 2e − 04 meaning that the p-value is statistically significant.

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
