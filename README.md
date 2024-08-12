# Music Genre Classification: Rock vs. Hip-Hop

![iphone_music](https://github.com/user-attachments/assets/cd63157e-62c1-433e-af66-04f826155716)

## Project Overview

This project focuses on classifying music tracks into two genres: Rock and Hip-Hop. The project was based on a guided exercise from Datacamp, with modifications and additional analysis done to enhance the learning experience. The goal was to build a machine learning model capable of accurately predicting whether a given track belongs to the Rock or Hip-Hop genre using audio features provided by the Echo Nest.

## Dataset

The project uses two datasets:

1. **fma-rock-vs-hiphop.csv**: Contains metadata and features for 17,734 tracks, including attributes like `track_id`, `bit_rate`, `composer`, `date_created`, `duration`, `genre_top`, and `title`. The `genre_top` column indicates the genre of each track, with labels "Rock" or "Hip-Hop".

2. **echonest-metrics.json**: Provides audio features for each track, such as:
   - `acousticness`
   - `danceability`
   - `energy`
   - `instrumentalness`
   - `liveness`
   - `speechiness`
   - `tempo`
   - `valence`
   
   These features were matched to the tracks using the `track_id` as a common key.

## Methodology

1. **Data Merging**: The `fma-rock-vs-hiphop.csv` and `echonest-metrics.json` files were merged using the `track_id` to create a single dataset containing both metadata and audio features.

2. **Exploratory Data Analysis (EDA)**: A thorough EDA was conducted to understand the distribution of features, handle any missing values, and visualize the relationships between different features and the target variable (`genre_top`).

3. **Modeling**:
   - Two machine learning algorithms were implemented:
     - **Logistic Regression**
     - **Decision Tree Classifier**
   - The models were evaluated using accuracy, precision, recall, and F1-score. Logistic Regression outperformed the Decision Tree Classifier in this task.

## Results

![download (5)](https://github.com/user-attachments/assets/96467764-7ceb-440a-a7f2-0b50509f74ba)

- **Logistic Regression** emerged as the better-performing model, providing more accurate predictions for classifying the music tracks into Rock or Hip-Hop genres.
- The final model can be used to predict the genre of new tracks based on their audio features.

## Credits

This project was inspired by and based on a guided exercise from DataCamp. The datasets used are sourced from the Free Music Archive (FMA) and Echo Nest.

## License

This project is licensed under the MIT License.
