# Anime Recommendation

The goal of repository is to create anime recommendation engine based on given rating by users. 
We will use collaborative filtering to predict anime that user most likely see based on previous anime rating of users.
The assumption of model is users have same watching behavior, probably like same other anime.

Data source: [Kaggle Anime Recommendations Database](https://www.kaggle.com/CooperUnion/anime-recommendations-database?select=rating.csv)

Training notebook: [![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1BncJGmCwiezahoeJYs2fHmf1tb9G84YD?authuser=1)

Similar anime playground: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/opalchonlapat/anime-recommend/835eb101f1b5f200e6d2df20c1bfae3d215cba3f?filepath=notebook%2Fsimilar_anime.ipynb)

## Evaluation

---

| Model                             | MAE     |
|-----------------------------------|---------|
| User median rating                | 1.00513 |
| User mean rating                  | 1.04116 |
| User mean without outlier rating  | 1.03732 |
| Anime median rating               | 1.08041 |
| Anime mean rating                 | 1.10887 |
| Anime mean without outlier rating | 1.10692 |
| Embedding Dot Bias Model          | 0.92832 |
| Neural Network Model              | 0.85407 |


## Usage

---

- [Anime_recommendation_dataset.ipynb](notebook/Anime_recommendation_dataset.ipynb): Jupyter notebook for training
- [similar_anime.ipynb](notebook/similar_anime.ipynb): Find similar anime from embedding
- [anime.zip](anime.zip): Dataset
- [models.pth](notebook/models/model.pth): Pre-trained model