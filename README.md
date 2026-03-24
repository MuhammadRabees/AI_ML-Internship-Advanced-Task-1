# AI_ML-Internship-Advanced-Task-1

## Objective of the Task
The goal of this project is to fine-tune a pre-trained transformer model (BERT) to automatically classify news headlines into specific topic categories. This task is part of the AI/ML Engineering Advanced Internship at DevelopersHub Corporation.

## Methodology / Approach
The project follows an end-to-end NLP pipeline:
* **Dataset:** Utilized the AG News Dataset available on Hugging Face Datasets. To optimize training time while maintaining performance, a smaller subset (2,000 training samples, 500 evaluation samples) was selected.
* **Preprocessing:** Tokenized and preprocessed the text data using the standard BERT tokenizer, ensuring padding and truncation for uniform sequence lengths.
* **Model Training:** Fine-tuned the `bert-base-uncased` model using the Hugging Face Transformers library.
* **Deployment:** Deployed the fine-tuned model using Gradio to create an intuitive, live interactive web interface directly within the notebook.

## Key Results or Observations
The model was evaluated using accuracy and F1-score metrics. Despite training on a significantly reduced dataset for just 3 epochs, the model achieved exceptional results:
* **Evaluation Accuracy:** 88.6%
* **Evaluation F1-Score:** 88.6%

**Observations:**
The identical accuracy and F1-score indicate a highly balanced model that performs consistently across all four news categories (World, Sports, Business, Sci/Tech) without bias. This demonstrates the powerful feature extraction and transfer learning capabilities of the `bert-base-uncased` architecture on text classification tasks.
