# Vertex AI Gen AI Evaluation

This notebook demonstrates how to use the Vertex AI Gen AI Evaluation SDK to evaluate the performance of large language models (LLMs).

The notebook covers the following topics:

- **Installation and Authentication**: Setting up the environment and authenticating with Google Cloud.
- **Evaluating a single model**: Performing evaluation using prebuilt metrics like TEXT_QUALITY, COHERENCE, FLUENCY, and GROUNDEDNESS.
- **Comparing multiple candidates**: Comparing the performance of two different models using pairwise evaluation.
- **LLM-based metrics**: Utilizing LLM-based metrics for evaluation.
- **Defining a custom metric**: Creating and using a custom metric for evaluation.
- **Computation-based and custom function metrics**: Demonstrating the use of computation-based metrics such as exact_match, bleu, and rouge_1.
- **Evaluating third-party models**: Evaluating models from other providers like OpenAI.
- **Visualizing results**: Visualizing the evaluation results using a radar chart.

This notebook provides a comprehensive guide to getting started with the Vertex AI Gen AI Evaluation SDK for evaluating your LLMs.


# Ragas Gen AI Evaluation

This notebook demonstrates how to evaluate the performance of a simple Large Language Model (LLM) application using the Ragas library. The evaluation process involves using various metrics to assess the quality of the LLM's responses.

The notebook begins by installing the necessary libraries, including `ragas`, `sacrebleu`, `rapidfuzz`, `rouge_score`, and `langchain-google-genai`.

It then introduces and demonstrates the use of several **non-LLM based metrics**:

- **BleuScore**: This metric compares the generated response to a reference text based on n-gram precision and a brevity penalty. It's a traditional metric often used in machine translation evaluation.
- **NonLLMStringSimilarity**: This metric measures the similarity between the response and reference using string distance algorithms like Levenshtein, Hamming, and Jaro. It's useful for evaluating direct text similarity without involving an LLM.
- **RougeScore**: This metric assesses the overlap between the generated response and the reference text using n-gram recall, precision, and F1 score. It's commonly used for evaluating summarization and translation tasks.
- **ExactMatch**: This simple metric checks if the generated response is an exact match to the reference text. It's useful for scenarios requiring precise output, such as tool calls.
- **StringPresence**: This metric checks if the generated response contains a specific reference string. It's helpful for verifying the inclusion of keywords or phrases.
- **AspectCritic**: This metric allows for evaluating responses based on predefined aspects described in natural language. The output is binary, indicating whether the response aligns with the defined aspect. Examples shown include evaluating "summary accuracy," "verbosity," and "maliciousness."

Overall, this notebook provides a practical introduction to using the Ragas library for evaluating LLM applications, covering both traditional and LLM-powered evaluation approaches.

## Author

* **Juan Guillermo Gómez**
* Linkedin: [@jggomezt](https://www.linkedin.com/in/jggomezt/)

## License

    Copyright 2025 Juan Guillermo Gómez

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS
