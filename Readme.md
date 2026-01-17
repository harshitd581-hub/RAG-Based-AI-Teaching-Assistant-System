
## basically (MY MODEL AIM)=
SUPPOSE  I log into my course, and basically what happens is that we have a lot of videos.
Now let’s assume that I want to ask an AI (like ChatGPT) a question such as:
“Where is NumPy Broadcasting taught?”
If I directly ask ChatGPT this question, it will not be able to tell me, because ChatGPT does not have access to my course videos.
And this is where Retrieval comes in — this is the brain of the system, which we call RAG (Retrieval-Augmented Generation).
This is what makes the system intelligent.
We have many videos and many lessons, and we need to feed this data smartly to the LLM in such a way that the LLM is able to understand what content is present where.
This is an AI-based system where we can ask questions like:
“In this course, where does NumPy Broadcasting start?”
And the system will tell us in which video number NumPy Broadcasting is explained.

## 📚 RAG-Based AI Teaching Assistant

An AI-powered teaching assistant that allows students to ask questions directly from course videos.The system converts videos into text, intelligently chunks the content, stores embeddings, and uses a Retrieval-Augmented Generation (RAG) pipeline to generate accurate answers from the relevant video segments.

## 🚀 Project Overview

In many online courses, content is spread across multiple long videos, making it difficult for students to quickly find answers.

This project solves that problem by:

Converting course videos into timestamped text

Creating semantic embeddings

Retrieving the most relevant video chunks

Generating context-aware answers using an LLM



# How to use this RAG AI Teaching assistant on your own data
## Step 1 - Collect your videos
Move a

## Step 2 - Convert to mp3
Convert all the video files to mp3 by ruunning video_to_mp3

## Step 3 - Convert mp3 to json 
Convert all the mp3 files to json by ruunning mp3_to_json

## Step 4 - Convert the json files to Vectors
Use the file preprocess_json to convert the json files to a dataframe with Embeddings and save it as a joblib pickle

## Step 5 - Prompt generation and feeding to LLM

Read the joblib file and load it into the memory. Then create a relevant prompt as per the user query and feed it to the LLM


