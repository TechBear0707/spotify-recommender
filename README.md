# spotify-recommender
A song recommendation system utilizing k-means clustering, PCA, and Spotify's API. Accesses a user's liked playlist and generates song recommendations. For the full article and main findings, you can visit [here]([https://developer.spotify.com/dashboard/applications](https://medium.com/@logan.margo314/building-a-spotify-song-recommender-using-k-means-clustering-15c8b4c84464))

## Features
- **Spotify API Integration**: Accesses your liked songs from your Spotify account to analyze your music preferences.
- **K-Means Clustering**: Groups songs into clusters based on audio features like danceability, energy, loudness, etc.
- **PCA**: Reduces the dimensionality of song features for easier visualization of the clusters.
- **Song Recommendations**: Recommends songs based on the cluster of your liked songs.

## Table of Contents
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Requirements
Make sure you have the following installed:
- Python 3.6+
- A Spotify developer account (to generate a client ID and client secret)
- Libraries such as: 
  - spotipy (for interfacing with Spotify's API)
  - pandas, numpy (for data handling)
  - scikit-learn (for clustering and PCA)
  - matplotlib, yellowbrick (for visualization)
Install the required libraries using the following command:
```bash
pip install -r requirements.txt
```
## Required Environment Variables
You will need to set up environment variables for Spotify API credentials:
- `CLIENT_ID`: Your Spotify client ID
- `CLIENT_SECRET`: Your Spotify client secret
- `REDIRECT_URI`: Your Spotify redirect URI
You can set these environment variables in your terminal or in a `.env` file in the root directory of the project.

## Installation
1. Clone the repository:
```bash
git clone https://github.com/TechBear0707/spotify-recommender.git
cd spotify-recommender
```
2. Install the required libraries:
```bash
pip install -r requirements.txt
```
3. Set up Spotify API credentials:
- Go to [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications) to create a new app.
- Add your credentials to the `.env` file:
4. Run the application:
```bash
python main.ipynb
```

## Usage
1. **Populate random songs**: Populates random songs from Spotify's API to create a dataset.
2. **Get user's liked songs**: Accesses your liked songs from your Spotify account.
3. **Analyze audio features**: Analyzes the audio features of the songs with respect to popularity and features over time.
4. **Cluster songs**: Groups songs into clusters based on audio features.
5. **Visualize clusters**: Visualizes the clusters using PCA.
6. **Get song recommendations**: Recommends songs based on the cluster of your liked songs.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
