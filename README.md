# AI-Restaurant-Analytics-Agent
An AI-powered restaurant analyst that transforms raw sales data into actionable business insights, inventory forecasts, and automated visual reports using LangChain and Gemini 2.0.


## Overview: This solution is an AI-powered analytics agent that empowers restaurant managers to query sales data using natural language. It acts as a bridge between raw data and operational strategy, transforming complex spreadsheets into clear, actionable insights.

## How it Works: The system leverages a LangChain agent integrated with a Pandas DataFrame and the Gemini 2.0 Flash LLM. It dynamically writes and executes Python code to compute metrics, manipulate data, and perform time-series comparisons directly from the dataset.

## Key Capabilities: To provide specialized restaurant intelligence, I integrated custom Python tools:

- Inventory Forecaster: Predicts next week’s product demand and calculates specific ingredient requirements based on recent sales trends.

- Sales Visualizer: Generates comprehensive monthly reports featuring automated charts for revenue trends, product performance, and weekday distributions.

## Reliability & Precision: 
Driven by a strict system prompt, the agent is grounded in business logic. It automatically interprets the latest date as "today," enforces professional formatting, and ensures every response is data-backed and formatted for immediate executive decision-making.
