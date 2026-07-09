# [Week 6 - Language](https://cs50.harvard.edu/ai/weeks/6/)

## Progress
- Completed lecture [2026-06-21]
- Completed project Parser [2026-06-22]
- Completed project Attention [2026-06-29]

## Key Concepts
- **Text Prediction**: The task of predicting the next word or token based on the previous context. However, even if a model can generate grammatically correct sentences, the output may not always be meaningful or logically coherent.
    - **Context Free Grammar**: A formal grammar system that describes how sentences can be broken down into syntactic components, such as nouns, verbs, noun phrases, and verb phrases.
    - **n-gram**: A sequence of n words or tokens. For example, a unigram contains one token, a bigram contains two tokens, and a trigram contains three tokens. n-grams can be used to model word patterns and estimate the probability of a word appearing after a given sequence.
    - **Tokenization**: The process of splitting text into smaller units, usually words or tokens. Although humans can naturally recognize words in a sentence, computers often need text to be cleaned and processed first, such as removing punctuation or filtering out tokens that do not contain alphabetical characters.
- **Text Classification**: The task of assigning text to a category, such as identifying whether a sentence expresses positive or negative sentiment.
    - **Bag-of-words Model**: A text representation method that focuses on which words appear in a document, without considering word order or grammar.
    - **Naive Bayes Classifier**: A probabilistic classifier that can be used for text classification. It learns which words are more likely to appear in each class, such as positive or negative sentiment, and uses those probabilities to classify new text.
        - **Smoothing**: A technique used to avoid assigning zero probability to words that were not seen during training.
- **Word Representation**: A method for converting words into numerical vectors so that they can be processed by machine learning models and neural networks.
    -**One-hot Representation**: A representation where each word is assigned a unique vector, with one position set to 1 and all other positions set to 0. However, this approach becomes inefficient when there are many words, and it does not capture similarities between words.
    -**Distribution Representation**: A representation where words are mapped to vectors based on the contexts in which they appear. Words with similar meanings tend to appear in similar contexts, so they are represented by similar vectors. For example, “dinner” and “breakfast” may appear near similar words, so their vector representations may be close to each other.

- **Text Translation**: The task of converting text from one language into another. One architecture used for this task is the encoder-decoder model. The encoder processes the input sequence and produces a hidden-state representation that summarizes the input. The decoder then uses this representation to generate the output sequence in the target language, one token at a time.

- **Attention**: A mechanism that allows a model to focus on the most relevant parts of the input when producing an output. Instead of treating every word as equally important, attention helps the model assign different levels of importance to different words depending on the context.

- **Transformer**: A neural network architecture that uses self-attention to process tokens in parallel rather than strictly sequentially. Because transformers do not process words one at a time in order, they use positional encoding to preserve information about word order. Transformers are especially important in modern natural language processing and are also used in other areas such as computer vision, audio, and multimodal AI.


## What I've Learned
I found context-free grammar especially interesting because it made me think about sentence structure in a way I had not considered before. When I learned English as a second language, I studied grammar as a human learner, but I did not think deeply about how a computer might represent grammar. Humans can often understand meaning, tone, and missing context naturally, but computers need language to be represented in a more structured and numerical form.

This week helped me see why natural language processing is so complex. Words need to be tokenized, represented numerically, and interpreted in context. Even a simple sentence can involve grammar, word meaning, sentence structure, and ambiguity. When this problem is expanded across thousands of words and many different languages, the scale becomes difficult to imagine. It gave me a greater appreciation for machine translation systems and the amount of work behind them.

I was also excited to finally learn about transformers. I had heard the term many times before, but I did not understand what it meant in AI. I now understand that transformers use attention mechanisms to process tokens in parallel while still preserving information about word order through positional encoding. I am still curious whether transformers are mainly useful for language tasks or whether the same architecture can be applied to other types of data. This is something I would like to explore through further reading.


## Challenges
The projects were not as technically difficult as some earlier CS50 AI projects because they relied more heavily on existing libraries. However, the Attention project was still valuable because it required me to interpret model behavior instead of only implementing an algorithm. Analyzing attention heads helped me think more carefully about what a model might be learning internally, while also reminding me that attention patterns are not always easy to interpret.


## Next Step
- Start CS50 Cybersecurity to get a little bit introduction to cybersecurity knowledge. And maybe it would be my future career path. Then at that time, I would wanna work on CompTIA or some other certificates. And don't forget to look into HTB for practice and OSSU for more peripheral knowledge about this subject.
- Courses from [OSSU Core Security](https://github.com/ossu/computer-science#core-security) will be the next next things I look into after finishing CS50 Cybersecurity and only if I am interested in this area. I kinda feel like I would because I love solving puzzles.
    - [Cybersecurity Fundamentals by RIT](https://www.edx.org/learn/cybersecurity/rochester-institute-of-technology-cybersecurity-fundamentals)
    - [Principles of Secure Coding by UC Davis](https://www.coursera.org/learn/secure-coding-principles)
    - [Identifying Security Vulnerabilities by UC Davis](https://www.coursera.org/learn/identifying-security-vulnerabilities)
    - [Identifying Security Vulnerabilities in C/C++Programming by UC Davis](https://www.coursera.org/learn/identifying-security-vulnerabilities-c-programming)
