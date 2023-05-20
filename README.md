# How Can We Compare Song Audio Files and Classify them?

## Research Question
Since we’ve never worked with audio data or classification of audio data we wanted to try working with data that is structured as such. 
We ask the question: how do the audio features from songs, specifically Spotify Tracks compare to each other? 

Is there a relationship between the some of these features such as tempo correlating with danceability/energy/liveness and if so how are they correlated. Additionally, how can we use these features to cluster songs based on these audio tracks of songs being coverted to numeric features?

## Hypothesis
Certain audio features will be statistically different between the distribution of certain genres. 

For example, the mean "tempo" of Pop Artists will be higher than that of Ballad Singers since Pop songs tend to be more upbeat and fast. 

If numerical data is extracted from the songs then models can be trained to cluster / classify songs into different groups since there will be enough difference between certain features between certain groups. This approach of comparing audio features between two groups can then be applied to other projects such as comparisons of living beings/objects to classify the two.

## Table of Contents

1. [Overview](#overview)
2. [Requirements](#requirements)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Further Applications](#further-applications)
6. [Contributors](#contributors)

## Overview

This project consists of the following components:

1. Audio Feature Extraction: We extract audio features on the Top Charting Songs from Spotify's API
2. Deep Learning Model: We create a deep learning model using TensorFlow and Keras to classify songs into genres and listening personas.
3. Evaluation: We evaluate the model's performance using accuracy, precision, recall, and F1-score metrics.
4. Adaptability: The project is designed to be easily adaptable for other audio classification tasks.

## Requirements
- Python 3.8+
- librosa
- TensorFlow
- Keras
- NumPy
- pandas
- scikit-learn
- Optional: Cuda (if training on an Nvidia GPU)

## Installation
To install the project and its dependencies, follow these steps:

1. Clone the repository:

```
git clone https://github.com/COGS108/Group_Sp23_The_group_chat
```

2. Change to the project directory:

```
cd Group_Sp23_The_group_chat
```

3. Install the required dependencies:

```
pip install -r requirements.txt
```

## Usage

To use this project for classifying audio clips, follow these steps:

1. Prepare your data: Scape the dataset from Spotify's API or directly download it manually.

```
python extract_audio_features.py 
```

3. Train and evaluate the model: Run the `train_and_evaluate.py` script to train the deep learning model and evaluate its performance:

```
python train_and_evaluate.py --input_file input_file.csv
```

## Further Applications

This project can be easily adapted to other audio classification tasks, such as:

- Identifying speakers in a conversation
- Detecting emotions in speech
- Recognizing animal sounds or bird calls

To adapt the project, simply prepare your data and follow the usage instructions outlined above.

## Contributors

- [Nate del Rosario](https://natdosan.github.io)
- [Lisa Hwang](https://github.com/lisasunhwang)
- [Mateo Ignacio](https://github.com/mjignacio)
- [Geovaunii D. White](https://github.com/geovaunii)
- [Samuel Piltch](https://github.com/samuelpiltch)

We appreciate all contributions to this project. If you would like to contribute, please open an issue or submit a pull request on the project's GitHub repository.

This is your group repo for your final project for COGS108.

This repository is private, and is only visible to the course instructors and your group mates; it is not visible to anyone else.

Template notebooks for each component are provided. Only work on the notebook prior to its due date. After each submission is due, move onto the next notebook (For example, after the proposal is due, start working in the Data Checkpoint notebook). 

This repository will be frozen on the final project due date. No further changes can be made after that time.

Your project proposal and final project will be graded based solely on the corresponding project notebooks in this repository.

Template Jupyter notebooks have been included, with your group number replacing the XXX in the following file names. For each due date, make sure you have a notebook present in this repository by each due date with the following name (where XXX is replaced by your group number):

- `ProjectProposal_groupXXX.ipynb`
- `DataCheckpoint_groupXXX.ipynb`
- `EDACheckpoint_groupXXX.ipynb`
- `FinalProject_groupXXX.ipynb`

This is *your* repo. You are free to manage the repo as you see fit, edit this README, add data files, add scripts, etc. So long as there are the four files above on due dates with the required information, the rest is up to you all. 

Also, you are free and encouraged to share this project after the course and to add it to your portfolio. Just be sure to fork it to your GitHub at the end of the quarter!
