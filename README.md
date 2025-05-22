## Recruitment Coding Challenge: AI/ML & Ops - KnowDroids.AI

This assignment is designed to give you an opportunity to showcase your skills in a way that aligns with your interests and strengths. You'll be able to choose from development routes (Time Series ML or AI Search) and then have the option to enhance your project with operational tasks.

We encourage you to select tasks and a depth of implementation that best demonstrates your abilities. We understand the nature of time constraints, that's why quality and thoughtfulness are valued over completing every single optional item.

---

### General Requirements for Submission:

1.  **GitHub Repository:** All your code, an informative `README.md`, and any necessary data/model files (or clear instructions on how to obtain them) should be in a public GitHub repository (or a private one shared with us).
2.  **README.md:** Your README should include:
    *   Setup instructions (dependencies, environment variables, etc.).
    *   How to run/use your project (e.g., commands, API endpoints).
    *   A brief explanation of your model validation approach (for the Time Series route).

**Extra Info:**
- We will provide an OpenRouter API key for access to various LLMs if your chosen tasks require it. To receive the key, or if you have any questions during the assignment, please contact Filip Sikora at filip.sikora@knowdroids.ai.
- For any deployment tasks, feel free to use free tiers on platforms like Vercel, Render, Hugging Face Spaces, or any other service you're comfortable with.
- Preferred Language to use is Python.
- Preferred toolkit for handling LLMs is [LangChain](https://www.langchain.com/).

---

### Pick a Primary Route

Select a primary development route. After completing the core tasks for your chosen route, you can enhance it with the "Optional Common Enhancements" listed further below. (No one's stopping you from trying them both.)

#### Route 1: The Time Series Specialist & LLM Integrator

Develop an end-to-end time series analysis solution with an LLM-powered interface.

1.  **Core Task: Time Series Model Development & Validation**
    *   **Dataset:** Choose a **time series dataset** of your interest. Publicly available datasets are preferred for ease of review (e.g., stock prices, weather data, sensor readings, economic indicators, IoT device data). *Provide a link to or include the dataset in your repository.*
    *   **Modeling:** Prepare the data and fit **one** appropriate machine learning model to it. Your task is to either:
        *   **Predict** future values of the time series (forecasting).
        *   **Classify** segments or characteristics of the time series (e.g., anomaly detection, pattern classification like "peak," "trough," "stable").
    *   **Validation:** Include a validation of your fitted model. Justify your choice of model, task (prediction/classification), and validation strategy in your README.

2.  **Core Task: LLM Agent for Model Interaction**
    *   Prepare a simple agent using an LLM of your choice (e.g. OpenRouter) that can "handle" your fitted time series model.
    *   "Handling" means the LLM agent should be able to:
        *   Accept input relevant to your chosen task (e.g., "Predict the next 7 days of stock X," or "Is the recent pattern in sensor Y anomalous given this historical data?" potentially through natural language queries or structured input).
        *   Pass this data/query to your trained time series model for inference.
        *   Receive the prediction or classification output from your model.
        *   Present or interpret the inferred data back to the user (e.g., in natural language, a clear structured format, or perhaps even describing a generated plot).
    *   *Example (Prediction):* A user might ask the LLM agent, "What's the predicted sales volume for next month given the past year's data?" The agent then uses the time series model to get the prediction and replies.
    *   *Example (Classification):* A user might ask, "Analyze the ECG data for the last 5 minutes. Is there an arrhythmia present?" The agent uses the model to classify the segment and replies.

---

#### Route 2: The AI Search & Retrieval Specialist

Build a semantic search engine, with options to expand its capabilities.

1.  **Core Task: Semantic Textual Search Engine**
    *   Choose a corpus of text documents (e.g., a collection of articles, product descriptions, book excerpts, your own notes).
    *   Implement a semantic textual search engine. This typically involves:
        *   Generating embeddings (you can use LLMs for this via OpenRouter, or other embedding models like Sentence-Transformers).
        *   Storing these embeddings.
        *   Allowing a user to input a query, generate an embedding for the query, and retrieve the most semantically similar documents from your corpus.

2.  **(Optional) Enhancement: Multi-Modal Search Engine**
    *   Extend your search engine to handle multi-modal data (e.g., text and images).
    *   Queries could be text-to-image, image-to-text, or image-to-image.

3.  **(Optional) Enhancement: RAG on Top**
    *   Implement a simple Retrieval Augmented Generation (RAG) system using your search engine.
    *   Your system should retrieve relevant documents/chunks using your semantic search and feed these retrieved contexts along with the original question to an LLM (via OpenRouter) to generate a comprehensive answer.

---

### Optional Common Enhancements (Applicable to your chosen route)

Once you've completed the tasks of your chosen route, you can further enhance your project with any of the following:

1.  **Web Application Wrapping:**
    *   Wrap your solution (Time Series model + LLM agent, or Search Engine) into a simple web application.
    *   Consider using frameworks like FastAPI (for APIs), Streamlit (for interactive web apps), Gradio, or even a simple command-line interface (CLI).

2.  **Containerization:**
    *   Containerize your application using Docker. Provide a `Dockerfile` and, if applicable, `docker-compose.yml`.

3.  **Deployment:**
    *   Deploy your wrapped and/or containerized application and expose it via a public URL.
    *   As mentioned, services like Vercel, Render, Hugging Face Spaces, or similar free-tier options are excellent for this.

---

### Submission:

Please submit the solution including a link to your GitHub repository within 2 weeks from starting by emailing it to **Filip Sikora at filip.sikora@knowdroids.ai**.

If you have any questions during the assignment, please don't hesitate to reach out to **Filip Sikora at filip.sikora@knowdroids.ai**.

Good luck, and we look forward to seeing what you build!
