# article-summarizer-NLP-44-620
Web Mining and Applied NLP

See [BeautifulSoup Quickstart Guide](https://www.crummy.com/software/BeautifulSoup/bs4/doc/#quick-start)

Choose a BeautifulSoup parser:

- 'html.parser' (default, you get this with BeautifulSoup)
- 'html5lib' (install separately if desired)

## Getting Started

Fork (copy into your GitHub account) and clone down (to your machine) this repo to get started with web scraping.

## Requirements

    beautifulsoup4          # parsing webpages (HTML documents)
    html5lib                # parsing webpages (HTML documents)  - especially if poorly formatted
    ipykernel               # for Jupyter notebooks
    jupyterlab              # for Jupyter notebooks
    matplotlib              # customizing visualizations
    requests                # make HTTP requests (a very popular Python package)
    spacy                   # for NLP 
    spacytextblob           # for NLP - combines spaCy and TextBlob (simpler interface)

## 1. Virtual Environment Management (Windows PowerShell)

1. **Create a virtual environment**
   ```powershell
   py -m venv .venv
   ```

2. **Activate the virtual environment**
   ```powershell
   .\.venv\Scripts\activate
   ```

3. **Upgrade pip, setuptools, and wheel**
   ```powershell
   py -m pip install --upgrade pip setuptools wheel
   ```

4. **Install required packages**
   ```powershell
   py -m pip install --upgrade -r requirements.txt
   ```

---

## 2. Running Python Scripts

```
- Activate your `.venv` and ensure all required packages are installed.
- Verify all external packages in your scripts are listed in `requirements.txt`.
```
---

## 3. Repeatable Workflow Checklist

When resuming work on your project, follow these steps:

1. [Pull latest changes](https://github.com/denisecase/pro-analytics-01/tree/main/03-repeatable-workflow)
2. Activate virtual environment
3. Install dependencies
4. Run Python scripts
5. Modify and test code
6. Add, commit, and push changes to Git

---

## 4. Git Add-Commit-Push CheatSheet

```powershell
git clone https://github.com/youraccount/yourrepo
git add .
git commit -m "custom message"
git push -u origin main
git pull origin main
git push
```

## # Final Project: Article Summarizer

Complete the tasks in the Python Notebook in this repository.
Make sure to add and push the pkl or text file of your scraped html (this is specified in the notebook)

## Rubric Final Project: Article Summarizer

* (Question 1) Article html stored in separate file that is committed and pushed: 1 pt
* (Question 2) Polarity score printed with an appropriate label: 1 pt
* (Question 2) Number of sentences printed: 1 pt
* (Question 3) Correct (or equivalent in the case of multiple tokens with same frequency) tokens printed: 1 pt
* (Question 4) Correct (or equivalent in the case of multiple lemmas with same frequency) lemmas printed: 1 pt
* (Question 5) Histogram shown with appropriate labelling: 1 pt
* (Question 6) Histogram shown with appropriate labelling: 1 pt
* (Question 7) Cutoff score seems appropriate given histograms: 2 pts (1/score)
* (Question 8) Summary contains a shortened version of the article (less than half the number of sentences): 1 pt
* (Question 8) Summary sentences are in the same order as they appeared in the original article: 1 pt
* (Question 9) Polarity score printed with an appropriate label: 1 pt
* (Question 9) Number of sentences printed: 1 pt
* (Question 10) Summary contains a shortened version of the article (less than half the number of sentences): 1 pt
* (Question 10) Summary sentences are in the same order as they appeared in the original article: 1 pt
* (Question 11) Polarity score printed with an appropriate label: 1 pt
* (Question 11) Number of sentences printed: 1 pt
* (Question 12) Thoughtful answer based on reported polarity scores: 1 pt
* (Question 13) Thoughtful answer based on summaries: 1 pt

## The following sites might help find information to work with - or just search the web or ask your favorite AI assistant for ideas based on your own unique interests.

   Shakespeare https://shakespeare.mit.edu/ 
   Music APIs https://www.jsonapi.co/public-api/category/Music
   Twitter API https://developer.twitter.com/en/docs/twitter-api
   Spotify API https://developer.spotify.com/documentation/web-api
   NLP Datasets https://github.com/niderhoff/nlp-datasets
   Kaggle Reddit Dataset https://www.kaggle.com/datasets/pavellexyr/reddit-r-nonewnormal-dataset
   Kaggle Twitter Datasets https://www.kaggle.com/search?q=kaggle+twitter
   Kaggle Song Lyrics Datasets https://www.kaggle.com/datasets/deepshah16/song-lyrics-dataset

## Export notebook to HTML

   1. Use JupyterLab (or Jupyter Notebook) to export your .ipynb files as HTML. Try either:
      Using the Jupyter menu: File -> Save and Export As... -> HTML
   2. !jupyter nbconvert --to html name_of_notebook.ipynb
   3. import os
      os.system('jupyter nbconvert --to html yourNotebook.ipynb')

## package installed

Had to install the English model: py -m spacy download en_core_web_sm

## Project Overview

~~~
✅ Web Scraping - Successfully fetched Hamlet's full text (175,084 characters) from MIT's Shakespeare website
✅ Sentiment Analysis - Analyzed overall sentiment: Polarity 0.1573 (positive) with 2,529 sentences
✅ Token Analysis - Found top 5 tokens: hamlet (469), lord (306), king (202), horatio (156), o (123)
✅ Lemma Analysis - Found top 5 lemmas: hamlet (469), lord (306), king (204), horatio (156), come (146)
✅ Sentiment Histograms - Created visual distributions showing most sentences are neutral (-0.1 to 0.1)
✅ Summary Generation - Created both token-based (612 sentences) and lemma-based (619 sentences) summaries
✅ Comparative Analysis - Both summaries showed higher positive sentiment (0.33) than the original (0.16)
~~~