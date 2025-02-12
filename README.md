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
