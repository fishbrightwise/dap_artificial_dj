## dap_artificial_dj
The assumption for either path is that you have Anaconda and Jupyter Notebook installed on your device.

### Just the Recommender without the Data Engineering:
This is for users who want to try out our emotion to song recommender!
There is no need to extract and engineer any of the data as the necessary files will be provided in the download folder.

#### How to use:
1. Please download the Built Model from https://drive.google.com/file/d/1YfaT1fePQwKcm6zlofu9S9STbMeITake/view?usp=sharing. Extract the .zip file and place everything in the extracted folder into your kernel environment folder location.

2. Run Notebook "1_input_generation.ipynb" and input the respective information when prompted. For information on how to obtain the necessary keys: https://github.com/fishbrightwise/dap_artificial_dj

3. Once you have filled in all the required inputs, Notebook 1_input_generation.ipynb will proceed to run "2_", "3_" and "4_" in order.

4. If all goes smoothly, nearing the end of "4_recommender_model.ipynb", you should be re-directed to a Spotify Authentication Page. Click allow, but do not close the page yet.

5. Once the page has changed to a seemingly blank one, copy the URL webpage link of that page. If you did not make any changes to the Spotify API settings, it should begin with "localhost" or some version of that. Copy this link and input it in the 4. when prompted to.

6. Once the whole process is completed, you should be able to see your new playlist with recommended songs in your very own account.

7. When you are done. You may delete the "token.txt" file. It contains your Spotify account information. If you leave it in and someone else uses your version of this model. The playlists they get recommended will be created in your Spotify account instead.

### Constructing the Recommender Model:
This is for users who want to modify and create their variants of this model from scratch.

#### How to use:
1. Please download/install the following:
    - Spotify 600K dataset from https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks?resource=download.
    - Emotion Detection dataset from https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp/data.
    - The Recommender Engineering/construction notebooks from https://drive.google.com/file/d/1DpacejAJOdlkdyyo1u7Fs9fMGWNE0fYO/view?usp=sharing.
    Also, obtain the necessary keys from Spotify from the links below.

2. Add the .csv files into the "data" folder and the notebooks into the main folder.

3. Run "0.1_data extraction.ipynb" from top to bottom on python with an environment kernel. Input the spotify information accordingly where needed. "tracks_with_genres.csv" should be craeted in the "data" folder. This should generate "tracks_with_genres_&_language.csv" file in the "data" folder.

4. Run "0.2_clustering.ipynb" from top to bottom to generate "tracks_with_genres_lang_emotion.csv" file in the "data" folder.

5. Lastly, run "0.3_genre_lang_extraction.ipynb" from top to bottom to receive "extracted_languages.csv" and "extracted_superset_genres.csv" files in your "data" folder.

6. Now, the model is ready to be used.

7. From this point onwards, you can follow the Built Model's steps to achieve the final output.

8. When you are done. You may delete the "token.txt" file. It contains your Spotify account information. If you leave it in and someone else uses your version of this model. The playlists they get recommended will be created in your Spotify account instead.

### Library used:
1. Spotipy Library: https://spotipy.readthedocs.io/en/2.22.1/

2. Spotify Language Scraper: https://pypi.org/project/spotify-lyrics-scraper/

3. Language Detection (langdetect): https://pypi.org/project/langdetect/

4. Emotion Detection Dataset: https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp/data

### Frameworks Used:
To install them onto your environment: pip install xxx in the terminal, or create a new code cell in any of the notebooks and %pip install xxx.
1. Pandas
2. Numpy
3. Matplotlib
4. Seaborn
5. Scikit-learn
6. Ast
7. Tensorflow
8. Spotipy
9. LangDetect
10. Spotify-Lyrics-Scraper
11. JSON
12. NLTK
13. Random

### Spotify API and Account Keys Manual:
1. Spotify API Client Key and Secret: https://developer.spotify.com/documentation/web-api

2. Spotify sp_dc & sp_key: https://pypi.org/project/spotify-lyrics-scraper/#obtaining

### Installation referrences:
1. Anaconda: https://docs.anaconda.com/free/anaconda/install/index.html

2. Jupyter Notebook: https://jupyter.org/install

3. Creating a Conda Environment: https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#activating-an-environment
