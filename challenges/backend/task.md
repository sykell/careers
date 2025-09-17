# Test task

## Introduction

This test task is for the backend developer position.
While your primary responsibility will be backend development, you will also have to be able to work on frontend applications.

This exercise has two goals:

* **For us:** To evaluate your production-quality code, API design reasoning, and overall development approach.
* **For you:** To experience the day-to-day work at Sykell through a realistic project.

## Code and project ownership

This is purely an exercise; we have no intention of using your submission in production.
You retain full ownership of your work and may license it as you see fit.
If you choose not to move forward with us, you’re free to open-source it or include it in your portfolio.

## Areas of focus

We will evaluate your submission on:

* **Backend requirements**
    * Usage of Go (Golang) (MUST)
    * Usage of framework of your choice (e.g., Gorm, Gin, Echo, etc.) (OPTIONAL)
    * Usage of MySQL for data storage (MUST)

* **Front-end**
    * UI must be a React Web application (MUST)
    * TypeScript (MUST)

* **General**

    * Reproducible builds (use your preferred vendoring/packaging system)
    * Code structure and organization
    * Consistent error handling and reporting (no crashes under non-critical conditions)
    * API request to backend must use authorization mechanism
    * Show a chain of commits representing project progression, including initial scaffolding, incremental feature additions, and any refactoring steps
    * Automated backend tests covering few happy-path scenarios
    * Total implementation time should not exceed 8 hours (feel free to spread this across multiple days)

> **Note:** As this role is backend focused, the quality and completeness of your Go code will carry greater weight.

# Task Description

Build a web application that accepts a website URL as input, crawls it and displays key information about that page.

**Back-end data collection (per URL):**

* HTML version
* Page title
* Count of heading tags by level (H1, H2, etc.)
* Number of internal vs. external links
* Number of inaccessible links (those returning 4xx or 5xx status codes)
* Presence of a login form

**Front-end requirements (high → low priority):**

1. **URL Management**

    * Add URLs for analysis
    * Start/stop processing on selected URLs

2. **Results Dashboard**

    * Paginated, sortable table (columns: Title, HTML Version, #Internal Links, etc.)

3. **Real-Time Progress**

    * Display crawl status for each URL (queued → running → done / error)

# How to submit test task

1. Create a **public GitHub repository** and commit your code there.
2. Include a **README.md** with clear instructions how to build and run your application.
3. Email the repository link to **[careers@sykell.com](mailto:careers@sykell.com)**.


# Evaluation criteria (scorecard)

| **Criterion**                   | **Description**                                                                    | **Weight** | **Score (1–5)** | **Weighted Score** | **Comments** |
|---------------------------------|------------------------------------------------------------------------------------|-----------:|----------------:|-------------------:|--------------|
| **1. Front-End Implementation** |                                                                                    |        10% |                 |                    |              |
| • React & TypeScript Quality    | Clarity, modularity, use of hooks, TS typing discipline                            |        10% |                 |                    |              |
| **2. Back-End Implementation**  |                                                                                    |        50% |                 |                    |              |
| • Go Code Quality               | Readability, error handling, idiomatic use of Go                                   |        25% |                 |                    |              |
| • Testing (happy paths)         | Coverage of core flows; meaningful assertions                                      |         5% |                 |                    |              |
| • MySQL Schema & Data Access    | Logical schema design; safe queries; migrations or seed scripts                    |        15% |                 |                    |              |
| • Reproducible Builds           | Vendoring/packaging consistency (e.g. modules, Dockerfile)                         |         5% |                 |                    |              |
| **3. Core Features**            |                                                                                    |        30% |                 |                    |              |
| • URL Ingestion & Crawl Control | Add URLs, start/stop processing                                                    |         5% |                 |                    |              |
| • Data Collection Accuracy      | Correct detection of HTML version, headings, link counts, login form, broken links |        20% |                 |                    |              |
| • Authorized API Calls          | Proper auth mechanism in requests                                                  |         5% |                 |                    |              |
| **4. Documentation & Setup**    |                                                                                    |        10% |                 |                    |              |
| • README & Run Instructions     | Completeness and clarity of setup steps                                            |         5% |                 |                    |              |
| • Code Organization & Comments  | Logical project structure, helpful inline comments, small isolated commits         |         5% |                 |                    |              |
| **TOTAL**                       |                                                                                    |       100% |                 |                    |              |
