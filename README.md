## Sentiment Analysis and Text Summarization of Flipkart Mobile Phone Reviews with Recommendation System 📱📊

### Overview 
This project performs sentiment analysis and text summarization on mobile phone reviews scraped from Flipkart, combined with a recommendation system based on product data 🛒. It leverages NLP techniques, machine learning, and data visualization to provide insights into customer opinions and suggest relevant products 👍👎.

### Features 
*   **Data Scraping:** Scraped data of over 4800 mobile phones 📱, including reviews, ratings ⭐, prices 💰, and review counts from Flipkart using Selenium.
*   **Data Cleaning and EDA:** Comprehensive data cleaning and exploratory data analysis (EDA) to prepare the data for analysis and recommendation 🧹.
*   **Recommendation Engine:** A recommendation system is built using numerical data and cosine similarity ⚙️.
*   **Sentiment Analysis:** Sentiment scores generated for reviews using transfer learning with transformer pipelines 😊😞.
*   **Text Summarization:** Implementation of text summarization to extract key insights from customer reviews 📝.
*   **Machine Learning Models:** Trained machine learning models for sentiment analysis, achieving 85-92% accuracy 🤖.
*   **Data Storage:** Recommendation matrices, sentiment scores, and summaries are stored for efficient read operations 💾.
*   **UI and Flask Application:** A user interface (UI) and Flask application for easy interaction and visualization 🖥️.
*   **Data Visualization:** A Tableau dashboard for visualizing data insights 📈.

### Technologies Used 
*   **Selenium:** For web scraping 🌐.
*   **Pandas, NumPy:** For data cleaning and EDA 🐼.
*   **Scikit-learn:** For machine learning models 🧠.
*   **Transformers (Hugging Face):** For sentiment analysis and text summarization 🤗.
*   **Flask:** For creating the web application 🧪.
*   **Tableau:** For data visualization 📊.

**Run the application:**

    ```
    python project.py
    ```

### Data Collection 
1.  **Scraping Flipkart:**
    *   Used the Selenium script to scrape mobile phone reviews and data from Flipkart 🖱️.
    *   Stored the scraped data in a structured format (e.g., CSV) 🗄️.

### Data Preprocessing 
1.  **Cleaning the Data:**
    *   Removed irrelevant data and handled missing values 🗑️.
    *   Performed EDA to understand data distribution and patterns 🔍.
2.  **Feature Engineering:**
    *   Created features for the recommendation engine using numerical data ✨.
    *   Prepared text data for sentiment analysis and summarization ✍️.

### Sentiment Analysis and Text Summarization 
1.  **Sentiment Score Generation:**

    ```
    from transformers import pipeline
    pipeline_sentiment_classification = pipeline('sentiment-analysis', device=0)
    ```
2.  **Text Summarization:**

    ```
    import torch
    from transformers import pipeline
    summarizer = pipeline("summarization", model="facebook/bart-large-cnn", device=0)
    ```
3.  **Model Training:**
    *   Trained ML models on the generated sentiment scores 💪.
    *   Achieved 85-92% accuracy depending on the model ✅.
4.  **Data Storage:**
    *   Stored sentiment scores and summaries for efficient access 📚.

### Recommendation System 
1.  **Recommendation Matrix:**
    *   Generated a recommendation matrix using cosine similarity 👯.
    *   Stored the matrix in a CSV file 📊.

### UI and Flask Application 
1.  **Flask Setup:**
    *   Created a Flask application to serve the UI ⚙️.
2.  **UI Development:**
    *   Developed a user interface to interact with the recommendation system and sentiment analysis results 💻.

### Data Visualization 
1.  **Tableau Dashboard:**
    *   Created a Tableau dashboard to visualize key insights and metrics 📈.

### Usage 
1.  **Running the Flask Application:**
    *   Execute the `project.py` file to start the Flask application ▶️.
    *   Access the UI through a web browser 🌐.
2.  **Using the Recommendation System:**
    *   Enter user preferences to get mobile phone recommendations 💯.
    *   View sentiment analysis results and summaries for each product 📝.

### Challenges and Future Enhancements 
*   **Resource Limitations:** Due to limited resources and time, model training for text summarization was not completed 🚧.
*   **Future Enhancements:**
    *   Train a model for text summarization 🚀.

### Credits 
*   [Flipkart](https://www.flipkart.com/) for providing the mobile phone review data 🙏.
*   [Hugging Face Transformers](https://huggingface.co/transformers/) for the sentiment analysis and text summarization pipelines 🙌.
*   [Tableau](https://www.tableau.com/) for data visualization 🤝.
