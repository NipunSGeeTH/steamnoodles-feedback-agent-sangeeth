## SteamNoodles Feedback Agent

This project provides a feedback analysis and response generation system for the SteamNoodles restaurant chain. It leverages sentiment analysis and generative AI to process customer feedback, visualize sentiment trends, and generate professional responses.

### Features
- **Sentiment Analysis**: Classifies feedback as positive or negative using HuggingFace's DistilBERT model.
- **Response Generation**: Uses Google Gemini (Flash) to generate empathetic, professional replies to customer feedback.
- **Visualization**: Plots sentiment distribution from customer reviews using Matplotlib.

### How It Works
1. **Install Dependencies**: The notebook installs required packages (`pandas`, `matplotlib`, `transformers`, `torch`, `google-generativeai`).
2. **Load Data**: Reads customer reviews from `restaurant_reviews.csv`.
3. **Analyze Sentiment**: Classifies each review as positive or negative.
4. **Generate Responses**: For each feedback, generates a short, friendly response using Gemini.
5. **Visualize Trends**: Plots a bar chart of sentiment distribution for the last 7 days.

### Usage
1. Open the notebook: `steamnoodles-feedback-agent.ipynb`
2. Run all cells to install dependencies, load data, and execute the analysis and visualization.
3. Update the path to your `restaurant_reviews.csv` if needed.

### Example
```python
feedback = "The noodles were amazing, but the staff was rude."
response_info = system.generate_response(feedback)
print("Feedback:", response_info["feedback"])
print("Sentiment:", response_info["sentiment"])
print("Response:", response_info["response"])
```

### Requirements
- Python 3.8+
- Jupyter Notebook
- API key for Google Gemini (replace in the notebook)

### File Structure
- `steamnoodles-feedback-agent.ipynb` — Main notebook for analysis and demo
- `restaurant_reviews.csv` — Sample customer feedback data
- `README.md` — Project documentation

---
**Note:** The Gemini API key in the notebook is a placeholder. Replace it with your own for full functionality.
