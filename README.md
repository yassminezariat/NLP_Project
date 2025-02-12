# NLP_Project
* *Big Idea* <br/>
Inequalities arising from health deficiencies : Dyslexia
The need to promote programs and assistive technologies that aim to help and assist children in their lecture activities.

* *Essential Question* <br/>
How can we promote and implement effective programs and assistive technologies to support children with dyslexia in their learning activities?

* *Challenge* <br/>
Reducing Educational Inequalities for Children with Dyslexia through Programs and Assistive Technologies in Lecture Activities.

> [!IMPORTANT]
> Health and Education

* health problems account for approximately 20% of the reasons why children fail to complete primary school (World Health Organization).

* 30% worldwide of the elementary school population is struggling with reading (Unesco 2021).
 

* 15% to 20% of students has a language based learning disability (Dyslexia Center of Utah).

 * 70% - 80% of people with poor reading skills are likely to be dyslexic (Dyslexia Center of Utah).

> [!IMPORTANT]
> WHAT IS DYSLEXIA ?  <br/>
Dyslexia is a learning disorder that affects a person's ability to read, write, and spell. It is a neurological condition that can make it difficult for individuals to process language, which can result in problems with reading fluency, accuracy, and comprehension.

> [!TIP]
>Generating Guiding Questions

* what is the impact of this disability on the individual ?  <br/>
Experience difficulties with phonological processing, working memory and attention. 

* What are current best practices for identifying dyslexia in children and adults ?  <br/>
Comprehensive evaluation that includes assessment of reading and writing abilities, phonological processing, working memory and attention.

* How can technology be used to support individuals with dyslexia ?   <br/>
The use of : Text-to-speech , Speech-to-text (AudioBooks), Text Summarization


**Dataset**
I leveraged web scraping to collect the data, preparing it for the next steps.
Books in children's literature (sorted by population) and free kids books : <br/>
![image](https://github.com/user-attachments/assets/2684e563-093d-4f9e-999d-ff2cbaeab42b)
 <br/>
 
**Modeling**  <br/>

1.**VOSK** <br/>
![image](https://github.com/user-attachments/assets/8b290b69-9bae-4b1e-b393-131f7dc35f23)
 <br/>
 * Vosk supports multiple neural network architectures, including LSTM and transformer models, and offers pre-trained models for several languages,including English, Spanish, French, German, Italian, Portuguese, Russian, Turkish, and Chinese. These models can be used for offline speech recognition, meaning that the speech data is processed locally on the user's device, rather than being sent to a remote server for processing. This can be useful for applications that require fast and reliable speech recognition, such as voice-controlled assistants or transcription tools. <br/>

* In addition to the pre-trained models, Vosk also provides tools for training custom models on specific datasets. This can be useful for applications that require speech recognition for specialized domains or languages that are not included in the pre-trained models. Overall, Vosk is a powerful and flexible toolkit for building speech recognition applications. <br/>
> [!IMPORTANT]
> We can download Vosk model from "https://alphacephei.com/vosk/models" <br/>


2.**T5** <br/>
![image](https://github.com/user-attachments/assets/bc3270ff-e210-4687-893c-4dcbeb502f44)<br/>

* Transformer-based model architecture with addition of a text-to-text framework It casts various NLP tasks into a text-to-text format, where both the input and output are represented as text.

* T5  utilizes a token masking mechanism called "Masked Language Modeling" (MLM) to enhance the model's learning. This mechanism involves masking certain words in the input text and training the model to predict these masked words.

* Various variants : T5-small, T5-based, T5-large, T5-3b, T5-11b 

* Model used : 
T5-small60 million parameters 6 layers of encoder 6 layers of decoder each encoder and decoder layer contains 8 self-attention heads

3.**Pre-fine tuning T5 for Keyword extraction** <br/>
4.**Reducing resources with Pruning** <br/>
5.**Text summarization with transformer :  Pegasus** <br/>
![image](https://github.com/user-attachments/assets/617376f9-137e-4060-9b99-d0388d19c62f) <br/>
-its main task is to predict missing or masked words in a sentences .

- employs an encoder-decoder architecture

- the encoder takes in the input and processes it to create a representation to captures the contextual information of the text 

-the decoder generates the summary based on this encoded representation

-based on attention mechanism (self-attention) 

-the model is already fine-tuned on a specific sum tasks

-during inference : 

beam search algorithm  explore multiple potential summary sequences.

Iterative refinement : strategy to improve the quality of the generated summary
<br/>
6.**Evaluation of bart + T5 + Pegasus + GPT2 for text summarazation :** <br/>

**Web Application**  <br/>
![Image](https://github.com/user-attachments/assets/ab8fb693-1dbc-4cbb-9c15-6131c9bfb0b1)

![Image](https://github.com/user-attachments/assets/b7da78b2-5e22-4932-8658-26a39c349d58)

![Image](https://github.com/user-attachments/assets/ee1eadf8-8c22-40e8-bdf1-f555d80a6fb5)
