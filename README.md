# Natural-Language-Processing-Projects

### Langchain

- **Imports Necessary Libraries**: Used LangChain and Hugging Face Hub to interact with pre-trained language models.
- **Defines Prompt Template**: Created a PromptTemplate for generating responses to user-defined questions, specifying placeholders for questions and answers.
- **Initializes Language Model**: Used the HuggingFaceHub class to load the **Bloom** model for generating text responses, with adjustable parameters like temperature and maximum response length.
- **Handles Multiple Questions**: Defined a list of questions related to sports and measurements.
- **Generates Answers**: Iterated through the list of questions, using the LLMChain to generate answers for each question based on the defined prompt template.
- **Displays Results**: Printd each question along with the corresponding generated answer, demonstrating the model's ability to provide informative responses.
