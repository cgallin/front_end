# $${\color{purple}Cover Genie}$$
https://github.com/cgallin/cover_genie
## https://cover-genie.streamlit.app/

## This app generates cover letters written by ChatGPT through the OpenAI API.
   + A data set of current job postings in several Canadian cites was generated through [Jobs API](https://rapidapi.com/Pat92/api/jobs-api14)
   + A [DistilBERT](https://huggingface.co/docs/transformers/en/model_doc/distilbert) NLP model was trained on a [Kaggle dataset](https://www.kaggle.com/datasets/arshkon/linkedin-job-postings) to classify job postings into the top 11 industries.
   + The classifier model was used to classify and filter the jobs scraped by Jobs API.
   + The user's CV (in .pdf format) is uploaded and they choose a job title, location and preferred industries.
   + Using cosine similarity the filtered job postings are narrowed down to five by relevance to the uploaded CV.
   + Cover letters for the top 5 jobs are then generated by an [OpenAI GPT model](https://platform.openai.com/docs/models) through OpenAI's API.
      
https://github.com/user-attachments/assets/d0d6c890-7dbf-46b0-a2d7-2549f1704a11

## DistilBERT Classifier 


## Cosine-Similarity Recommender 

## Langchain Model
