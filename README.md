# Topic Modeling for Apollo Hospital: LDA vs HDP

## Project Overview
This project focuses on analyzing social media content by and interactions with **Apollo Hospital** using advanced **topic modeling** techniques, specifically **Latent Dirichlet Allocation (LDA)** and **Hierarchical Dirichlet Process (HDP)**. The aim is to uncover hidden themes within the text data and compare the performance of these models in identifying key customer concerns and sentiments.

## Objective
- To extract meaningful topics from customer feedback using LDA and HDP.
- To compare the **coherence** of LDA and HDP models in interpreting the text data.
- To provide actionable insights on common customer concerns and sentiments.

## Approach
1. **Data Cleaning**:
    - Text cleaning involved removing punctuation, stopwords, and tokenizing the text.
    - **Lemmatization** was performed to reduce words to their base forms.

2. **Topic Modeling**:
    - **LDA Model** was built with 5 topics.
    - **HDP Model** was used to automatically determine the number of topics.
    - **CountVectorizer** was applied to create a term-document matrix with 8751 unique terms.
  
3. **Model Evaluation**:
    - Coherence scores for model evaluation:
        - **LDA Coherence**: 0.4168
        - **HDP Coherence**: 0.6805
    - HDP showed higher coherence, suggesting better topic separation and interpretation.

## Key Insights
- **LDA Topics** included:
    - Topic 0: ['liver', 'india', 'apollo', 'health', 'covid19']
    - Topic 1: ['get', 'contact', 'team', 'share', 'please']
    - Topics related to healthcare services, customer service, and COVID-19 were identified.

- **HDP Model** provided more refined topics with better coherence, suggesting it is a superior model for this dataset.

## Results
- **Top Topics** revolved around healthcare services, COVID-19 responses, and customer interactions.
- HDP proved to be more effective in capturing nuanced customer concerns, as evidenced by its higher coherence score.

## Technologies Used
- **Python** (Pandas, NumPy, Scikit-learn, Gensim)
- **Topic Modeling**: Latent Dirichlet Allocation (LDA), Hierarchical Dirichlet Process (HDP)
- **Visualization**: PyLDAvis for interactive topic exploration

## Future Work
- Implement **dynamic topic modeling** to track changes in customer concerns over time.
- Explore BERT-based topic models for improved interpretability and performance.

