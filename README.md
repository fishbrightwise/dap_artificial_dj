## dap_artificial_dj

### How to use:
1. Please download the Spotify 600K dataset from https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks?resource=download if you would like to run the model from scratch. (Data Extraction and Recommender System) If you only want the recommender system, obtian it from https://drive.google.com/file/d/1gl_TvnBU1Pb02-_J17qe_EoWwK4IBpbj/view?usp=sharing.

2. Add the .csv files into the data/ folder.

3. Run "data extraction.ipynb" from top to bottom on python with an environment kernel. tracks_with_genres.csv should be craeted in the data/ folder.

4. Run "recommender model testing.ipynb" from top to bottom.

5. Pop ups should appear. Enter your desired song name to use to search for recommendations similar to it. Press Enter.

6. Then, enter the desired playlist name the model will name the created playlist on your Spotify account in the next pop up. Press Enter.

7. After that, enter the desired number of songs you want to be recommended to by the model. Press Enter.

8. Following that, enter your Spotify API Client Id, Client Secret, sp_dc and sp_key in the next 4 pop ups respectively. Refer to the links below for how to obtain these. Press Enter after each one.

9. If this is your first time using the model, you should be redirected to a Spotify Authentication page. Click 'Allow' and you will be directed to a 'localhost' page. Copy the URL of that page in full.

10. When you go back to the model, you should be prompted with another pop up. Paste the copied URL there. Press Enter.

11. Now just wait until the model has finished running until the end. When done, you should have your new playlist in your Sptify account!

12. When you are done. You may delete the "token.txt" file. It contains your Spotify account information. If you leave it in and someone else uses your version of this model. The playlists they get recommended will be created in your Spotify account instead.

### Library used:
1. Spotipy Library: https://spotipy.readthedocs.io/en/2.22.1/

2. Spotify Language Scraper: https://pypi.org/project/spotify-lyrics-scraper/

3. Language Detection (langdetect): https://pypi.org/project/langdetect/

### Spotify API and Account Keys Manual:
1. Spotify API Client Key and Secret: https://developer.spotify.com/documentation/web-api

2. Spotify sp_dc & sp_key: https://pypi.org/project/spotify-lyrics-scraper/#obtaining
