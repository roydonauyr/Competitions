# Introduction

In this repo, it contains all competitions I had taken part in before. But some codes are unavailable.

| Competition Name | Position | Application | Code Availability |
| ------------- | ------------- | ------------- | ------------- |
| CitiHackOver 2022  | 1st Place  | Wealth Buddy App | Available |
| Visa internal hackathon | 1st Place | Combination of solutions on instagram to boost promoting of offers| Unavailable | 
| Accenture Pitch Competition | 1st Place  | Bring your own food restaurant app | Unavailable |
| JunctionX Asia Hackathon | First Runner Up | Reflection website | Unavailable |
| Goldman ESG Competition | Finalist  | ESG investing application | Available |
| GIC CodeToImpact  | Participant  | Investment/Portfolio website | Available |

# 1. Wealth Buddy Web Application
![GitHub](https://img.shields.io/github/license/Interstellarkai/Eternals)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Interstellarkai/Eternals)
![GitHub repo size](https://img.shields.io/github/repo-size/Interstellarkai/Eternals)
![GitHub language count](https://img.shields.io/github/languages/count/Interstellarkai/Eternals)
![GitHub last commit](https://img.shields.io/github/last-commit/Interstellarkai/Eternals)

Wealth Buddy is an application built for CitiHackOver 2022 with the intention to positions Citi as the modern bank for wealth management solutions, to drive client acquisition and strengthen client relationships in the Asian market.

## Demo Video 
In this video, we will take you through a quick pitch for you to understand the context of our application, thereafter, we will do a live demonstration of our app, Wealth Buddy  
https://www.youtube.com/watch?v=LAqM7PtSQRQ

## Key Features
- Embedded Dashboards 
- [Stock price prediction built with FB's Prophet - Stock Price Predictor](https://github.com/Interstellarkai/WallStreetAI)
- AI chat built with Lex 
- [Portfolio optimization](https://github.com/ketan1741/Benjamin-Graham-and-Warren-Buffett-Model-Stock-Exchange-)

## Screenshots
<img width="700" alt="Screen Shot 2022-08-12 at 12 39 02 AM" src="https://user-images.githubusercontent.com/72592202/184189422-bed0b125-08c6-407f-b5a6-1eda98b45def.png">
<img width="700" alt="Screen Shot 2022-08-12 at 12 42 07 AM" src="https://user-images.githubusercontent.com/72592202/184189413-1f2d92fd-b0d2-41d3-80da-3346d856b746.png">
<img width="700" alt="Screen Shot 2022-08-12 at 12 38 51 AM" src="https://user-images.githubusercontent.com/72592202/184189426-809a74c9-02c0-487e-93a7-ce1af864c986.png">
<img width="700" alt="Screen Shot 2022-08-12 at 12 38 32 AM" src="https://user-images.githubusercontent.com/72592202/184189432-cb0c9b80-aeaf-4baf-a28c-71f7d0061736.png">

## Getting Started

Download or clone project from github:
```
$ git clone https://github.com/Interstellarkai/Eternals
```

## Install - Local

Frontend:
```
$ cd frontend
$ npm install
$ npm run start
```

Backend:
With project environment (pipenv recommended):
```
$ cd backend
$ pipenv install
$ pipenv shell
$ python3 app.py --host=0.0.0.0 --port=5555
```

Otherwise normal install prerequisites:
```
$ pip3 install -r requirements.txt
```

## Install - Docker (Preferred)

```
$ docker compose build
$ docker-compose up
```

## To Access page
```
http://0.0.0.0:3000/
```

## Support
If you like the work we do, show your appreciation by 'FORK', 'STAR' and 'SHARE'.

# 2. Goldman-Sach-ESG-Comp
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/roydonauyr/Goldman-Sach-ESG-Competition)
![GitHub repo size](https://img.shields.io/github/repo-size/roydonauyr/Goldman-Sach-ESG-Competition)
![GitHub language count](https://img.shields.io/github/languages/count/roydonauyr/Goldman-Sach-ESG-Competition)
![GitHub last commit](https://img.shields.io/github/last-commit/roydonauyr/Goldman-Sach-ESG-Competition)

Competition on ESG data modelling and predictions

We were tasked with designing a solution for ESG investing and transforming unstructured data into structured data.

# Our Solution
Using LDA and light gradient boosting we extracted ESG data from public sources and transformed unstructured data to well-curated data.

![image](https://user-images.githubusercontent.com/44868878/178102056-687b7836-18ce-466a-b00a-87553a199077.png)

Process flow for text lemmatisation :
1.Use a regular expression to remove any punctuations and lowercase text.
2.Visualise with WordCloud
3.Transform the textual data in a format to serve as an input for training a Latent
Dirichlet Allocation (LDA) model.
• Tokenising the text and removing ‘stopwords’
• Convert the tokenised object into a corpus and dictionary
4.Construct Bigram and Trigram Models
• Bigrams and Trigrams with two important arguments to Phrases model
(min_count and threshold)
5.Perform text lemmatisation keeping only nouns, adjectives, verbs, adverbs
6. Data transformation
• Create Dictionary with gensim corpora library with optional filtering of tokens
• Create Corpus with lemmatised text by converting document (a list of words)
into the bag-of-words format = list of (token_id, token_count) 2-tuples. Each
word is assumed to be a tokenised and normalised string

![image](https://user-images.githubusercontent.com/44868878/178102829-f9b63536-ecc9-4a2a-b1d8-f5dc1550e084.png)

After LDA has been performed, topics can be classified by investors so as to study important key words or phrases regarding company related ESG reports to help investors decide if the company would be a good investment

![image](https://user-images.githubusercontent.com/44868878/178103253-b968666a-2069-400a-b9e3-f734773c1032.png)

Step 2: Using Light Gradient Booster, investors can add in additional features to decide if the company has a category that investors are looking for. These categories can be set by investors and can be used to predict a companies report. Once all reports has been predicted, investors would be able to view which category the company is leaning towards and decide if the company would be a good investment.

![image](https://user-images.githubusercontent.com/44868878/178103014-a09033a5-fa41-4651-8773-74ec6ac42f58.png)

# Further Improvements:
1. Preprocessing texts by removing unnecessary characters, unicode
characters, headers and footers (definable by user).
2. Perform structured analysis on the suggested words to extend stop
words for removal (depending on the domain area).
3. Continuous improvement on the topic model with updates to minimise
data drifts, maintain model relevancy.
4. Explore other models (Probabilistic Latent Semantic Analysis,
Probabilistic Latent Semantic Analysis or lda2vec) and used them for
comparisons with LDA via gensim libraries.
5. Analyse and filter words before storing from derived topics
6. Compute distances (Hellinger, Kullback-Leibler, Jaccard) between
each topic clusters and group based on distances (centroids).
7. Improve on the ESG word data bank with more relevant documents.
8. Perform feature engineering to improve ESG predictions.
9. Optimal hyperparameters for the Multi-class Classifier.

# 3.CodeToImpact
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/roydonauyr/CodeToImpactNew)
![GitHub repo size](https://img.shields.io/github/repo-size/roydonauyr/CodeToImpactNew)
![GitHub language count](https://img.shields.io/github/languages/count/roydonauyr/CodeToImpactNew)
![GitHub last commit](https://img.shields.io/github/last-commit/roydonauyr/CodeToImpactNew)

## Project Description:
Building a website that summarizes the respective information:
1. Investments
2. Portfolio (Incorporated analytics and past trends)
3. Consumer markets


## Important details
.env content

NODE_ENV = development

PORT = 8000

MONGO_URI = mongodb uri

JWT_SECRET = abc123

Node version:

Make sure your node version is 16.x

## Development process
Work on new features on a new branch
Before commiting, make sure to check if there is linting errors and fixed it
Create a PR to main branch
Get one people to review your PR before merging
to run local development server
npm install

npm run dev

to run local frontend server
cd client

npm install

npm run start
