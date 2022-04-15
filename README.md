# Analysis of Spotify Million Playlist Dataset Challenge

## Purpose

## Tools Utilized 
- Python
  - Pandas Library
- Excel
- R

## Dataset Information

**Dataset Name:** Spotify Dataset 1921-2020, 600k+ Tracks | [Link to Kaggle Dataset](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks)

**Dataset Owner:** Yamac Eren Ay

**Source:** Spotify Web API

**Release Data of Latest Version:** April 2021

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
