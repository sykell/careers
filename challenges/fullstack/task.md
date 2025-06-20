# Test task

## Introduction

This is a test task for the Fullstack developer position which is FE focused.
This means that your primary focus will be on the frontend, but you will also be required to work with backend services.

This test task has the following goals:

- It helps us to understand what to expect from you as a developer, how you
write production code, how you reason about API design etc.

- It helps you get a feel for what it would be like to work at Sykell, as
this exercise aims to simulate our day-as-usual and expose you to the type
of work we're doing here.

## Code and project ownership

This is a test challenge, and we have no intent of using the code you've
submitted in production. This is your work, and you are free to do whatever
you feel is reasonable with it. In the scenario when you don't pass, you can
open source it with any license and use it as a portfolio project.

## Areas of focus

These are the areas we will be evaluating in the submission:

- UI must be a React Web application
    - UI must be responsive and work on mobile devices
    - UI must be written in TypeScript
- Backend must be written in Golang
- Data storage must be implemented using MySQL
- At the minimum, create FE tests for happy path scenarios.
- Make sure builds are reproducible. Pick any vendoring/packaging system that
will allow us to get consistent build results.
- Ensure error handling and error reporting is consistent. The system should
report clear errors and not crash under non-critical conditions.
- API request to backend must use authorization mechanism.
- During final interview we will discuss your solution and will be adding new features to it.
- Total coding hours should not take longer than 8 hours (but you can spread it across multiple days)

**As this is FE focused position, FE code will carry more weight in the evaluation.**

# Task Description

Create a web application which takes website URL as an input and provides general information about the contents of the page.

Data to be collected for each URL in backend:
- HTML Version
- Page Title
- HTML heading tags count by level
- Amount of internal and external links
- Amount of inaccessible links (inaccessible link is the one which returns 4xx or 5xx status code)
- If a page contains a login form

User over UI should be able to (requirements sorted by priority High → Low):

- Add URLs for processing
- Start/stop processing of selected URLs
- Results dashboard:
    - Table with sortable/paginated columns (Title, HTML Version, #Internal Links, etc.)
    - Column filters and a global search box (fuzzy or starts-with)
- Details view
    - Clicking a row opens a new page with:
        - A bar or donut chart of internal vs external links
        - A list of broken links (4xx/5xx) with status codes
- Bulk actions (checkbox selection):
    - re-run analysis or delete
- See Real-time progress
    - Show the crawl status of each URL (queued → running → done / error)

# How to submit test task

1. Create a public github repository and commit code in it
2. Provide a [README.md](http://readme.md/) in github repository with instructions how to run application
3. Send a link to the repository to [careers@sykell.com](mailto:careers@sykell.com)