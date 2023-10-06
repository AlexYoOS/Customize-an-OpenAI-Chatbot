# Customize-an-OpenAI-Chatbot
## _Showcase of an embeddings based customization approach of Chat-GPT_

![Add flower image here](mariia-shalabaieva-unsplash.jpg)


This **Generative AI Task** involves customizing OpenAI`s Large-Language-Model (LLM), there are **2 methods offered** for customization:

1. **Embeddings Customization:**

    - In this approach, you modify the model's token embeddings to adapt it to a specific task or domain. Token embeddings are the representations of words or subwords that the model uses as input.
    - You can update the embeddings of certain tokens or subword pieces to emphasize domain-specific vocabulary. For example, if you're fine-tuning ChatGPT for medical conversations, you might customize the embeddings for medical terms to make the model more knowledgeable about medical topics.
    - The rest of the model remains largely frozen, meaning the pre-trained weights are not updated during this process. Only the embeddings for specific tokens are adjusted.
    - Customizing embeddings is a less intensive form of fine-tuning and is typically used when there are limited data or computational resources.

2. **Fine-Tuning:**
    - Fine-tuning involves updating not just the embeddings but also the weights of the entire model, including its layers, attention mechanisms, and neural network parameters.
    - You fine-tune the model on a task-specific dataset by providing input-output pairs that correspond to your task. For example, if you want to fine-tune ChatGPT for sentiment analysis, you would provide it with text samples and their associated sentiment labels.
    - During fine-tuning, the model learns to generalize from the provided dataset and adapt its internal representations to better perform on the target task.
    - Fine-tuning is a more powerful approach but often requires a substantial amount of task-specific data to be effective. It also has the potential to forget or overwrite some of the general knowledge learned during pre-training.


## Structure and features of this showcase

- **Data Preprocessing**  This includes wrangling data, and minor text standardizations.
- **Creating Embeddings:** Embeddings are mathematical representations of words, phrases, or other data in a vector space. These vectors capture semantic relationships between elements, allowing algorithms to understand and work with textual or categorical data more effectively.
- **Custom Prompt Creation** Custom prompt creation refers to the domain-sepcific initial input or instruction tha is provided to the language model when a tailored response is wanted.
- **Completion** Completion refers to the output generated by the language model in response to your custom prompt. When a custom prompt is provided, the model completes it by generating a text response based on its understanding of the prompt and its pre-trained knowledge.


> The project outlines the key steps to customize an OpenAI-chatbot, choosing 1 of the 2 mentioned native measures as described above is a direct and cost effective approach of applying OpenAi´s LLM e.g. as an in-house consultant, without the need of a third party service that applies a business framework on top of an OpenAI LLM API. However, the latter may be a suitable approach depending on ease of implementaion, client business case and cost of service. 

## Tech

This application uses a number of open source projects to work properly:

- [Python](https://docs.python.org/3/) Core programming language in AI and Data Science
- [Numpy](https://numpy.org) - The fundamental package for scientific computing with Python
- [Pandas](https://pandas.pydata.org/docs/index.html) - Open source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools
- [OpenAI tiktoken](https://github.com/openai/tiktoken) - Fast BPE tokeniser for use with OpenAI's models.

