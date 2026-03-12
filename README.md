# ITAI2373-NewsBot-Midterm
Repo for NLP midterm files

System Workflow:

flowchart TD
    A([📰 Raw News Articles\nKaggle Dataset]) --> B

    MOD2["Module 2 — Preprocessing Pipeline"]
        B[Text Cleaning\nLowercase, punctuation, HTML removal] --> C
        C[Tokenization] --> D
        D[Stop Word Removal] --> E
        E[Lemmatization]
    end

    MOD3["Module 3 — TF-IDF Feature Extraction"]
        F[TF-IDF Vectorization\nParameter tuning] --> G
        G[Category-Specific\nTerm Analysis]
    end

    MOD4["Module 4 — POS Tagging"]
        H[POS Tagging\nNLTK / spaCy] --> I
        I[Grammatical Pattern\nExtraction & Cross-Category Analysis]
    end

    MOD5["Module 5 — Syntax & Semantics"]
        J[Dependency Parsing] --> K
        K[Syntactic Feature\nEngineering & Semantic Roles]
    end

    MOD6["Module 6 — Sentiment Analysis"]
        L[Article-Level\nSentiment Classification] --> M
        M[Emotion Tone\nAnalysis & Distribution]
    end

    MOD7["Module 7 — Classification"]
        N[Train Multiple Classifiers\nNaive Bayes, SVM, Logistic Regression] --> O
        O[Model Evaluation\n& Comparison] --> P
        P[Best Model Selection]
    end

    MOD8["Module 8 — Named Entity Recognition"]
        Q[Entity Extraction\nPERSON, ORG, GPE, DATE, MONEY] --> R
        R[Frequency Analysis\n& Relationship Mapping]
    end

    E --> F
    E --> H
    E --> J
    E --> L
    E --> N
    E --> Q

    G --> S
    I --> S
    K --> S
    M --> S
    P --> S
    R --> S

    OUT["📊 NewsBot Output"]
        S[Results Aggregation] --> T
        T[Visualizations &\nInsight Report]
    end

    style MOD2 fill:#dbeafe,stroke:#3b82f6
    style MOD3 fill:#fef9c3,stroke:#eab308
    style MOD4 fill:#dcfce7,stroke:#22c55e
    style MOD5 fill:#f3e8ff,stroke:#a855f7
    style MOD6 fill:#ffe4e6,stroke:#f43f5e
    style MOD7 fill:#ffedd5,stroke:#f97316
    style MOD8 fill:#e0f2fe,stroke:#0ea5e9
    style OUT fill:#f1f5f9,stroke:#64748b
