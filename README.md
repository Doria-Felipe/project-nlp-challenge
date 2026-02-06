![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# PROJECT | Natural Language Processing Challenge

Use NLP to identify whether a news headline is real or fake news.

[Task Descriptions and Project Instructions](hhttps://github.com/ironhack-labs/project-nlp-challenge)

## Project Results 
In this project, we processed the dataset `training_data_lowercase.csv` that contains labels and texts and explored different classifiers results:
- Built a workflow of NLP preprocessing.
- Trained 50+ models, our best model was the Lemm. NN-embedding with ~ 94% accuracy and ~97% gini.
- Scored the dataset `testing_data_lowercase.csv` with the BOW Logistic regression with ~93% accuracy and ~96% gini resulting on the file `predictions.csv`.


## Repository Folders and Files

Here is a short description of the folder and files available on the repository.

### Documents
**Group 2 - Natural Language Processing Challenge - Presentation Slides**  
G2_NLP_Presentation.ppt

### dataset

- **training_data_lowercase.csv:** The training dataset for our model.
- **testing_data_lowercase.csv:** The unlabeled dataset for validation.
- **predictions.csv:** The predictions. It is composed of a .csv file separated with `\t` and the text from `testing_data_lowercase.csv`. The first row is the labels our model predicted and the second is the original text. There are no headers.

### Notebooks  
- **Project3_G2_NLP**: Our workflow where we worked to obtain each model.

## 🧹 Jupyter Notebook Hygiene (Required)

This project uses **nbstripout** to ensure that **Jupyter notebooks are always committed without outputs or execution metadata**.

This keeps:
- Git history clean
- Pull requests readable
- Merge conflicts to a minimum

Notebook outputs should **never** appear in commits or pull requests.

---

### One-time setup (per developer machine)

Install `nbstripout` and register it with Git:

```bash
pip install nbstripout
nbstripout --install
```

This repository includes a .gitattributes file at the root level that applies nbstripout to all Jupyter notebooks.

```
*.ipynb filter=nbstripout
```

> **Note:** Your first commit after running a notebook may fail.
> This is expected — `nbstripout` has cleaned the file.
> Simply run `git add .` and commit again.