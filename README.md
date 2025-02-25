# Multilingual and Crosslingual Methods and Language Resources

This respository provides bonus exercises for the lecture Multilingual and Crosslingual Methods and Language Resources in the winter semester of 2024. 
<br><br>

***Exercise 1: Low-Rank Adaptation and Crosslingual Transfer for Linguistic Acceptability***
<br>
This project explores the application of **Low-Rank Adaptation (LoRA) to fine-tune XLM-R**, a large pre-trained multilingual language model, for the task of linguistic acceptability. LoRA enables **fine-tuning with limited resources, while crosslingual transfer enhances the model's adaptability to new languages**. These techniques are crucial for building NLP systems that can be deployed across diverse linguistic landscapes. The goal is to **improve the model's ability to identify grammatically correct and acceptable sentences in different languages**. Specifically, the project involves:
<br><br>
What has been done:
<br>
- Fine-tuning XLM-R on the English Corpus of Linguistic Acceptability (CoLA) dataset using LoRA.
- Evaluating the fine-tuned model's performance on English test data.
- Further fine-tuning the model on the German portion of the Multilingual Evaluation of Linguistic Acceptability (MELA) dataset.
- Evaluating the model's performance on German test data and assessing its zero-shot transfer capabilities to other languages.
<br><br><br>


***Exercise 2: Aligning Multilingual Embedding Spaces***
<br>
This project focuses on aligning multilingual embedding spaces, specifically using a **supervised method for aligning English and German word embeddings**. It **uses pre-trained fastText embeddings and a bilingual word list** to learn a mapping between the two languages' vector spaces. The main goal is to **improve cross-lingual natural language processing tasks by creating a shared embedding space** where words with similar meanings across languages are **located close to each other**. This enables tasks like cross-lingual word translation and analogy completion.
<br><br>
What has been done:
<br>
- Loading pre-trained fastText embeddings for both languages.
- Loading a bilingual word list from the MUSE project.
- Extracting aligned word vectors for words present in both embeddings and the word list.
- Using the Procrustes method to learn an orthogonal transformation matrix for mapping the English embeddings to the German embedding space.
- Applying the transformation matrix to align the English embeddings.
- Evaluating the aligned embeddings using word translation accuracy and cross-lingual analogy completion tasks.
