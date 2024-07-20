# MelodyMatch: Personalized Music Recommendations Based on Your Vibe

1. Data Loading and Preparation:
   - The project begins with loading a dataset containing various features of Spotify songs          using pandas.
   - Relevant features such as popularity, energy, valence, tempo, and genre are selected for        clustering.
   - The categorical feature 'track_genre' is encoded into numeric values using LabelEncoder to      facilitate clustering.

2. Feature Scaling:
   - To standardize the feature values, StandardScaler is used. This step ensures that all           features contribute equally to the clustering process by scaling them to a standard range.

3. Clustering and Evaluation:
   - KMeans clustering is performed with a range of cluster values to determine the optimal          number of clusters.
   - Two methods, the Elbow method and silhouette scores, are utilized to assess the clustering      performance and decide the best number of clusters.
   - The optimal number of clusters is determined based on these evaluations.

4. Visualization:
   - Scatter plots are generated to visualize the data distribution before and after                 clustering, allowing for an understanding of how clusters are formed.
   - The scatter plots illustrate the effectiveness of clustering in grouping similar songs          together.

5. Song Recommendation:
   - A function is created to recommend songs based on the features provided by the user and         the identified cluster centers.
   - This function calculates distances between the user's input and cluster centers to find
     the most appropriate cluster for recommendations.

6. GUI Development:
   - A graphical user interface (GUI) is built using Tkinter, allowing users to input their
     preferences and receive song recommendations.
   - The GUI includes fields for entering song features and a dropdown menu for selecting the
     genre.
   - Upon clicking the recommendation button, the application processes the input, performs
     clustering, and displays a list of recommended songs.
