# Natural-Language-Processing-Projects

### Transformers

- **Imports Transformers Library**: Utilizes the transformers library to access various NLP models through pipelines.
- **Sentiment Analysis**: Analyzes the sentiment of individual and multiple sentences, categorizing them as 'POSITIVE' or 'NEGATIVE' with associated confidence scores.
- **Zero-Shot Classification**: Classifies a given sentence into predefined categories without prior training, indicating the most relevant labels and their confidence scores.
- **Text Generation**: Generates text based on a given prompt using the text-generation pipeline, providing one or more sequences of text continuation.
- **Mask Filling**: Predicts and fills in masked words in a sentence using the fill-mask pipeline, returning possible replacements with confidence scores.
- **Named Entity Recognition (NER)**: Identifies and classifies named entities (e.g., persons, organizations, locations) in a given sentence, with associated confidence scores.
- **Question Answering**: Answers questions based on a provided context, returning the answer along with its confidence score and character positions.
- **Text Summarization**: Summarizes a longer passage into a concise summary, highlighting the main points.
- **Translation**: Translates text from French to English, demonstrating multilingual capabilities.

### Langchain

- **Imports Necessary Libraries**: Uses LangChain and Hugging Face Hub to interact with pre-trained language models.
- **Defines Prompt Template**: Creates a PromptTemplate for generating responses to user-defined questions, specifying placeholders for questions and answers.
- **Initializes Language Model**: The HuggingFaceHub class loads the **Bloom** model for generating text responses, which has adjustable parameters like temperature and maximum response length.
- **Handles Multiple Questions**: Defines a list of questions related to sports and measurements.
- **Generates Answers**: Iterates through the list of questions, using the LLMChain to generate answers for each question based on the defined prompt template.
- **Displays Results**: Prints each question and the corresponding generated answer, demonstrating the model's ability to provide informative responses.
