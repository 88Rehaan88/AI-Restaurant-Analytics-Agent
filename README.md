# AI-Restaurant-Analytics-Agent
This AI-powered analytics agent empowers restaurant managers to query sales data using natural language. By acting as a bridge between raw spreadsheets and operational strategy, the system leverages LangChain and Gemini 2.0 to deliver automated inventory forecasts, performance trends, and professional visual reports.

The system combines several advanced components:
-  LangChain Agent Framework for dynamic Python code generation and execution.
-  Gemini 2.0 Flash for high-speed, reasoning-heavy data interpretation.
-  Custom Tool Integration for specialized tasks like inventory forecasting and automated visualization dashboard.
-  Rule-Based System Prompting to enforce business logic, time-series accuracy, and professional formatting.

------------------------------------------------------------------------------
### The Problem:
In a fast-paced restaurant environment, managers often spend hours manually reviewing sales records, performing complex calculations for inventory, and estimating future product requirements for the coming weeks. This manual process is not only time-consuming but also prone to human error. Miscalculating demand or missing a subtle revenue trend can lead to costly overstocking or even potential loss.

------------------------------------------------------------------------------

### The Solution:
This agent acts as a 24/7 digital analyst that does the heavy lifting for you. Instead of navigating spreadsheets, you can simply ask questions in plain English. The agent performs all necessary calculations and provides deep, data-driven insights to assist you in making confident, data-backed decisions.

------------------------------------------------------------------------------

### Key Capabilities: 
To provide specialized restaurant intelligence, we integrated custom Python tools:

- Inventory Forecaster: Predicts next week’s product demand and calculates specific ingredient requirements based on recent sales trends.

<img width="800" height="800" alt="sales_report" src="https://github.com/user-attachments/assets/e187dc7f-3dd2-4722-b91e-c550d07f6569" />

------------------------------------------------------------------------------

- Sales Visualizer: Generates comprehensive monthly reports featuring automated charts for revenue trends, product performance, and weekday distributions.
  
<img width="950" height="450" alt="Screenshot 2026-02-10 022431" src="https://github.com/user-attachments/assets/6383f950-1dcc-4db7-8b3f-d468c15298d5" />

------------------------------------------------------------------------------

### Reliability & Precision:
Driven by a strict system prompt, the agent is grounded in business logic which ensures every response is data-backed and formatted for immediate executive decision-making.

------------------------------------------------------------------------------

### Future Improvements: 
- **Security & Production Safety:**
While this project uses ‘allow_dangerous_code=True’ for local execution. However, in a real company setting, I would move this to a "Sandboxed Environment" (a secure, isolated digital container). This ensures that the AI can perform calculations without any risk of accidentally accessing or damaging/deleting the rest of the company's private data. 

- **Conversational Memory:**
Integrating LangChain Memory would allow the manager to engage in multi-turn dialogues, enabling the agent to remember context from previous questions for more natural follow-up analysis. (e.g., "Why did that happen?" or "Compare that to the previous week") without needing to repeat the initial parameters, creating a more natural and efficient "analyst-manager" interaction.

- **Domain-Specific Fine-Tuning:** Fine-tuning the underlying LLM on specialized supply-chain, business related and restaurant management datasets would sharpen the agent’s ability to provide more nuanced business strategy recommendations beyond basic data math and insights.

- **Hour tracking:** iterations could ingest hourly transaction data. This would allow the agent to identify precise peak hours, enabling managers to make data-backed decisions regarding staff scheduling and kitchen prep-times.

- **Advanced Time-Series Forecasting:** Replacing basic trend analysis with sophisticated models such as Prophet or ARIMA would significantly improve the accuracy of sales predictions by accounting for seasonality and complex growth patterns.

- **Automated Data Ingestion:** In future iterations, we would implement automated data ingestion, connecting the agent directly to the restaurant’s or Inventory Management system via API. This would ensure the agent is always up-to-date with the latest transactions, allowing for "live" monitoring and more responsive decision-making.

------------------------------------------------------------------------------

### 7. Limitations:
- **Insight vs. Causality:** The model is exceptionally strong at providing data-backed insights (identifying what happened and when), but it struggles with deep causal reasoning. For example, it can detect a 20% drop in sales, but without external data, it cannot "reason" if that drop was due to a competitor's promotion, bad weather, or a local road closure.

- **Static Data:** The agent currently analyzes a static export of data, which lacks real-time knowledge of the restaurant's operations. This means it cannot provide insights on live inventory levels or immediate mid-shift trends without a manual file upload.

- **Reasoning Latency:** For extremely complex queries requiring multiple data transformations, the agent may hit max_iterations limits, requiring users to break down their requests into smaller, more manageable questions.




