# Loan-Counselor-Agent
An AI Agent for Loan Counseling for further abroad studies.# Loan Counselor Agent

An AI‑powered assistant that helps students and professionals navigate the complex process of applying for education loans to study abroad.  The agent asks about your target country, course, financial situation and preferences, then suggests suitable loan programs, explains eligibility criteria and breaks down interest rates and repayment plans.

## Features

- **Conversational interface:** interact via a chat‑style UI to get personalised advice on education loans.
- **Loan programme guidance:** receives your study details and recommends loans based on factors like university, course and loan amount.
- **Information on eligibility and documentation:** outlines collateral requirements, credit scores, co‑signers and necessary documents.
- **Interest and repayment estimates:** estimates monthly repayments and total payable amounts based on typical interest rates.
- **Extensible design:** built with a modular architecture to allow integration of new banks or loan providers.

## Technologies used

- **Python** – core programming language.
- **LangChain or other LLM wrapper** – handles prompt construction and connects to a large language model (Gemini/ChatGPT) to generate responses.
- **Flask / Streamlit** – provides a REST API or web interface for the chat experience.
- **dotenv** – manages API keys and environment variables.

## Getting started

1. **Clone the repository** and navigate into it:

   ```bash
   git clone https://github.com/deepalisachan04/Loan-Counselor-Agent.git
   cd Loan-Counselor-Agent
   ```

2. **Create a virtual environment** (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # on Linux/Mac
   venv\Scripts\activate    # on Windows
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Set your API keys**:  copy `.env.example` to `.env` and add your LLM API key (e.g., `GOOGLE_API_KEY` for Gemini or `OPENAI_API_KEY` for OpenAI).

5. **Run the application**:

   ```bash
   python app.py
   ```

   Then open http://localhost:5000 in your browser to start chatting with the agent.  (The URL and script name may differ if you expose a different interface – adjust accordingly.)

## Usage

Start a session and provide details about your intended course and destination.  For example:

```
User: I want to pursue a master’s degree in computer science in Germany.  What loan options do I have?
Agent: Based on your course and destination, you might be eligible for XYZ Bank’s education loan, which covers tuition and living expenses.  You may need a co‑signer and collateral for amounts over ₹20 lakhs…
```

The agent will return personalised suggestions and may ask follow‑up questions for more accurate recommendations.

## Future enhancements

- Integrate real‑time APIs from major banks to fetch current interest rates and loan schemes.
- Add EMI calculators and currency conversion tools.
- Provide downloadable PDF summaries of recommended loan options.
- Deploy the app on a cloud platform with authentication and user dashboards.

## License

This project is licensed under the MIT License – see the `LICENSE` file for details.
