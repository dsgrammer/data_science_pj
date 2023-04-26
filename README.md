# data_science_pj
My personal Data Science project to build my portfolio.

Iteration as of 2023/04/26
Current program flow:
1. Get latest info for my Liked Songs in Spotify
	"06_2022-12-12_favorited_songs.ipynb"
2. The resulting dataframe is saved as "fav_list.csv" in the output folder, and uploaded to PostgreSQL DB.
3. Get the audio-features for each track, save to .csv, and upload to DB.
	"08_2023-02-23_get_audio_features_from_db_df.ipynb"


Notes to self:
Need a way to only pull audio features for newly added tracks.
As the code currently is, the time to run is very slow.
maybe output a temp file containing a timestamp and read it in, adjusting the SQL SELECT to only grab data after that datetime.
