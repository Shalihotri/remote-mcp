# Modular Command Program (MCP): Remote Utilities Toolkit

## Overview

This repository contains a custom-built **Modular Command Program (MCP)**, a lightweight and extensible command-line tool designed for running specialized remote utilities. MCPs are typically structured to be composable, fast, and easy to integrate within automation pipelines or larger systems.

This MCP contains two key modules:
- 🏅 **Nobel Prize Checker**: Queries and returns Nobel Prize laureates based on category and year.
- 🌡️ **Temperature Checker**: Fetches real-time temperature data for a given location using external APIs.

## What is an MCP?

An **MCP (Modular Command Program)** is a structured CLI tool or framework built to:
- Modularly run multiple command-based utilities.
- Be extensible for new tools.
- Operate remotely or locally with consistent command interfaces.
- Simplify maintenance and usage by separating logic into discrete, purpose-built modules.

### Applications of MCPs:
- Automating frequently-used system tasks or data queries.
- Building developer or analyst toolkits.
- Streamlining CLI-based reporting and diagnostics.
- Integrating into CI/CD, cron jobs, or scripting frameworks.

## Modules in This MCP

### 1. Nobel Prize Checker
- **Input**: Category, Year
- **Output**: Laureates and their contributions
- **Use case**: Quick reference for historical Nobel data.

### 2. Temperature Checker
- **Input**: City name
- **Output**: Current temperature and weather conditions
- **Use case**: Real-time environmental awareness in automation or dashboards.

---

## Getting Started

```bash
uv venv
uv pip install -r requirements.txt
python main.py check-nobel --year 2022 --category physics
python main.py check-temp --city London
