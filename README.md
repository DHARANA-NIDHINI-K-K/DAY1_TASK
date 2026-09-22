# Day 1 - Comparing Chatbot, Rule-Based Workflow, and AI Agent

## Project Overview

This project compares three different approaches to solving the same private-data problem:

1. Plain Chatbot
2. Rule-Based Workflow
3. AI Agent

The goal is to understand how each approach works, what tools or data it uses, and what limitations it has.

## Scenario

The scenario used in this project is a private expense-tracking problem.

The private expense data is stored in `expenses.txt`.

The user asks:

> How much did I spend on food?

The three approaches solve this same problem in different ways.

## 1. Plain Chatbot

The plain chatbot mainly provides a response to the user's question.

It does not independently use tools to access the private expense file.

## 2. Rule-Based Workflow

The rule-based workflow follows predefined steps and conditions.

It reads the expense data, checks the category of each expense, and adds the amount when the category is `Food`.

No LLM is involved in this workflow.

## 3. AI Agent

The AI agent follows the idea:

**Agent = LLM + Tools + Loop**

The agent can interpret the user's request, use tools to access information, observe the results, and continue taking actions until the task is completed.

## Project Files

- `chatbot.py` - Plain chatbot
- `workflow.py` - Rule-based workflow
- `agent.py` - AI agent
- `expenses.txt` - Private expense data
- `analysis.md` - Detailed analysis and comparison
- `requirements.txt` - Project dependencies
- `Output/` - Screenshots of the three approaches

## How to Run

### Plain Chatbot

```bash
python chatbot.py
