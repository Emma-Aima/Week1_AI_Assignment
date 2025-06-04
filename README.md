# Cryptocurrency Investment Advisor Chatbot
**📌 Overview**
This Python-based chatbot provides cryptocurrency investment recommendations by analyzing two key factors:
- Profitability (price trends, market capitalization)
- Sustainability (energy efficiency, project viability)
The bot uses rule-based logic to match user queries with the most suitable cryptocurrencies from its database, offering clear explanations for each recommendation.

**✨ Features**
Core Functionality
Profitability Analysis:
- Evaluates coins based on price trends ("rising", "stable", "fluctuating")
- Considers market capitalization ("high", "medium", "low")

Sustainability Assessment:
- Rates energy consumption ("very low" to "high")
- Uses sustainability scores (1-10 scale)
- Evaluates project viability

Intelligent Query Handling:
- Understands natural language queries
- Recognizes synonyms (eco/green/sustainable)
- Provides balanced recommendations for generic queries

**User Experience**
- Interactive command-line interface
- Helpful prompts with example questions
- Detailed justification for recommendations
- Ethical disclaimer on every response

**🛠️ Technical Implementation**
Data Structure
crypto_db = {
    "Bitcoin (BTC)": {
        "price_trend": "rising",
        "market_cap": "high",
        "energy_use": "high",
        "sustainability_score": 4,
        "project_viability": "high"
    },
    # ... other cryptocurrencies
}

**Scoring Algorithms**
1. Profitability Score: Combines price trend and market cap metrics

2. Sustainability Score: Incorporates energy use, sustainability score, and project viability

3. Combined Score: Weighted sum for balanced recommendations

**🚀 How to Use**
1. Run the Python script
2. The bot will greet you with instructions
Ask questions like:
- "Which crypto is trending up?"
- "What's the most sustainable coin?"
- "What should I buy for long-term growth?"

Type "exit", "quit", or "bye" to end the session

**🔮 Sample Interactions**
a. You: Which crypto is trending up?
CryptoBot: Invest in Ethereum (ETH)! 📈 It has strong growth potential!
Details: Price trend is rising, Market cap is high

b. You: What's the most sustainable coin?
CryptoBot: Invest in Cardano (ADA)! 🌱 It's eco-friendly with excellent sustainability credentials!
Details: Energy use is low, Sustainability score is 9/10

⚠️ Disclaimer: Crypto is risky—always do your own research!

**📈 Potential Enhancements**
API Integration
# Example using CoinGecko API
import requests
def get_real_time_data(coin_id):
    url = f"https://api.coingecko.com/api/v3/coins/{coin_id}"
    return requests.get(url).json()

Advanced NLP
from nltk.tokenize import word_tokenize
from nltk.corpus import stopwords

def process_query(query):
    tokens = word_tokenize(query.lower())
    return [w for w in tokens if w not in stopwords.words('english')]

**Additional Metrics**
- Transaction speed analysis
- Developer activity tracking
- Community growth metrics
- Regulatory compliance status

**⚠️ Important Disclaimer**
This chatbot provides educational information only. Cryptocurrency investments carry substantial risk. Users should always:
- Conduct their own research
- Consult financial advisors
- Never invest more than they can afford to lose
The disclaimer appears automatically with every recommendation.

**📂 Project Structure**
/crypto-chatbot/
│── crypto_advisor.py      # Main chatbot implementation
│── README.md              # This documentation
│── requirements.txt       # Python dependencies

**🏁 Getting Started**
- Ensure Python 3.x is installed
- Clone the repository
- Run python crypto_advisor.py
- Begin chatting with the bot

For questions or contributions, please open an issue in the repository.

**Contributors:**
Ileogben Emmanuella Aimalohi - emmanuellaileogben@gmail.com
