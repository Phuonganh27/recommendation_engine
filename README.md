# Recommendations with IBM

## Project Motivation

Within the IBM Watson Studio, an expansive collaborative community ecosystem exists, encompassing articles, datasets, notebooks, and other AI and ML assets. Users within this platform interact with these assets, offering a rich opportunity to enhance their experiences by connecting them with the most relevant resources.
This project has been undertaken to personalize the user experience through the development of a recommendation system.

## Introduction

This project focuses on the analysis of user interactions with articles within the IBM Watson Studio platform.
The aim is to suggest new articles that users are likely to find appealing.
Below, you can find an example of what the dashboard could resemble, displaying articles within the IBM Watson Platform.
![Example Dashboard](dashboard.png)

While the dashboard above currently showcases the most recent articles, the project aims to create a recommendation model to offer articles highly relevant to specific users.

The project is structured into the following sections:

### I. Exploratory Data Analysis

This section provides basic statistics about the dataset.

### II. Rank Based Recommendations

The section creates recommendations by simply identifying the most popular articles, primarily determined by the number of interactions.
Given the absence of article ratings, articles with the highest interactions are assumed to be the most popular, making them suitable recommendations for new users or anyone.

### III. User-User Based Collaborative Filtering

To offer more tailored recommendations to IBM's platform users, we adopt a user-user collaborative filtering approach. This method involves identifying users who exhibit similarities in their interactions with articles. Subsequently, articles that these similar users have engaged with can be recommended to one another.

### IV. Matrix Factorization

The project concludes with the implementation of a machine learning-based approach to recommendations. Utilizing the user-item interaction data, a matrix decomposition is constructed. This decomposition allows us to predict new articles that an individual may interact with, even though the predictive accuracy may be imperfect.

## Repository File Structure

The structure of this repository is organized as follows:

- The `data/` directory contains the necessary datasets for the project.
- `Recommendations_with_IBM.ipynb` is the Jupyter Notebook that contains the project code and analysis.
- This `README.md` file provides an overview of the project and its structure.

## Prerequisites

- Python (NumPy, Pandas)
- Jupyter Notebook
- Additional libraries, as specified in the project notebook

## Acknowledgments

We extend our gratitude to IBM Watson Studio for providing the dataset and the platform for this project.

## License

This project is released under the MIT License. Please refer to the [LICENSE](LICENSE) file for details.

## Author

- [Dang Phuong Anh](https://github.com/Phuonganh27)
