# Natural-Language-Processing-Projects

## Transformers

- **Imports Transformers Library**: Utilized the transformers library to access various NLP models through pipelines.
- **Sentiment Analysis**: Analyzed the sentiment of individual and multiple sentences, categorizing them as 'POSITIVE' or 'NEGATIVE' with associated confidence scores.
- **Zero-Shot Classification**: Classified a given sentence into predefined categories without prior training, indicating the most relevant labels and their confidence scores.
- **Text Generation**: Generated text based on a given prompt using the text-generation pipeline, providing one or more sequences of text continuation.
- **Mask Filling**: Predicted and filled in masked words in a sentence using the fill-mask pipeline, returning possible replacements with confidence scores.
- **Named Entity Recognition (NER)**: Identified and classified named entities (e.g., persons, organizations, locations) in a given sentence, with associated confidence scores.
- **Question Answering**: Answered questions based on a provided context, returning the answer with its confidence score and character positions.
- **Text Summarization**: Summarized a longer passage into a concise summary, highlighting the main points.
- **Translation**: Translated text from French to English, demonstrating multilingual capabilities.



## Langchain

- **Necessary Libraries**: Used LangChain and Hugging Face Hub to interact with pre-trained language models.
- **Prompt Template**: Created a Prompt Template for generating responses to user-defined questions, specifying placeholders for questions and answers.
- **Language Model**: The HuggingFaceHub class loaded the **Bloom** model for generating text responses, which had adjustable parameters like temperature and maximum response length.
- **Handling Multiple Questions**: Defined a list of questions related to sports and measurements.
- **Answer Generation**: Iterated through the list of questions, using the LLMChain to generate answers for each question based on the defined prompt template.
- **Results Display**: Printed each question and the corresponding generated answer, demonstrating the model's ability to provide informative responses.



## Question Answering on Squad Dataset

#### Data Preprocessing:

- Tokenized questions and contexts with AutoTokenizer from Hugging Face, implementing truncation and stride for large contexts.
- Prepared training examples by calculating start and end token positions for each answer.
- Processed validation examples similarly to maintain consistency for evaluation.

#### Model:

- Fine-tuned the BERT model (specifically bert-base-cased) for the question-answering task.
- Implemented the Trainer class from Hugging Face for efficient training.

#### Training Methodology:

- Configured training with specified hyperparameters (e.g., learning rate, epochs).
- Employed mixed precision training using fp16 for faster performance.
- Evaluated model performance after each epoch using Exact Match and F1 score metrics.

#### Results:

- Achieved an **Exact Match** score of approximately **81.18**% and an **F1 score** of about **88.67**% on the validation dataset.

#### Inference:

- Utilized a question-answering pipeline to predict answers from a given context, demonstrating the trained model's capability in a practical scenario.
