# FoodHub AI-Powered Food Delivery Chatbot

An intelligent, AI-powered customer support chatbot designed for **FoodHub**, a leading food aggregator company. This project automates real-time order tracking, manages customer queries, and connects directly to the company's order database using an SQL agent while maintaining safety through robust input and output guardrails.

---

## 📋 Table of Contents
- [Business Context](#business-context)
- [Objective](#objective)
- [Data Description](#data-description)
- [Project Architecture & Features](#project-architecture--features)
- [Author](#author)

---

## 💼 Business Context

The volume of online food delivery orders is growing rapidly among students, working professionals, and busy families. Customers frequently require real-time assistance regarding:
* Delivery times and order statuses
* Payment confirmations and details
* Return, replacement, and cancellation policies

Historically, these inquiries were managed manually by customer support teams, causing long wait times, inconsistent replies, and high operational overhead. FoodHub aims to bridge this gap by automating standard interactions using structured database queries and intelligent natural language processing.

---

## 🎯 Objective

1. **AI-Powered Automation**: Build a functional chatbot that interacts smoothly with customers in a polite, concise, and professional tone.
2. **Database Integration**: Leverage a LangChain SQL agent to securely connect with the order management database and fetch accurate transaction and tracking details.
3. **Safety & Guardrails**: Implement strict input and output guardrails to prevent system misuse, handle prompt injections gracefully, and seamlessly escalate complex issues to human customer support agents.

---

## 📊 Data Description

The chatbot interacts with an order management database featuring columns such as:
* `order_id`: Unique identifier for each transaction/order.
* `cust_id`: Unique customer identifier.
* `order_time`: Timestamp when the order was placed.
* `order_status`: Current lifecycle status (e.g., *placed*, *preparing*, *out for delivery*, *delivered*).
* `payment_status`: Payment verification and confirmation details.
* `item_in_order`: List or count of food items in the order.
* `preparing_eta`: Estimated preparation time.
* `prepared_time`: Actual timestamp when order preparation concluded.
* `delivery_eta`: Estimated delivery timestamp.
* `delivery_time`: Actual timestamp when order was delivered.

---

## 🛠️ Project Architecture & Features

* **LLM Integration**: Powered via LangChain and Groq-hosted language models for fast, context-aware conversational reasoning.
* **SQL Agent**: Translates natural language customer queries into optimized SQL queries to query live order details safely.
* **Guardrail Validation**: Ensures responses remain strictly within the domain of FoodHub operations and safeguards against erratic inputs.
* **Agent Orchestration**: Utilizes **LangGraph** to manage multi-step reasoning and escalation flows.

---

## 👤 Author

* **Tharun Ganapathi**  
* *Submission Date*: October 18, 2026
