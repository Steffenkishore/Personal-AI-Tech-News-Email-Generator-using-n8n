# 📰 Personal AI & Tech News Email Generator using n8n + Gemini + SERP API

An AI-powered News Automation system built using `n8n`, `Google Gemini`, `RSS Feeds`, `SERP API`, and `Gmail`.

This automation collects the latest AI news, tech updates, and live AI event information from multiple sources, summarizes everything using AI, and delivers a clean personalized newsletter directly to email.

---

# 🚀 Features

- Fetch AI news from multiple RSS feeds
- Collect latest tech updates automatically
- Discover live AI events using SERP API
- Summarize news using Google Gemini AI
- Send daily AI newsletter to email
- Fully automated workflow using n8n
- Real-time information aggregation

---

# 🛠️ Tech Stack

- Automation : n8n
- AI Model : Google Gemini
- News Sources : RSS Feeds
- Search API : SERP API
- Email Service : Gmail
- API Integration : HTTP Request Node

---

# 📌 Workflow Architecture

```text
Schedule Trigger →
RSS Feed News →
SERP API Search →
Merge Data →
Aggregate Content →
Gemini AI Summary →
Gmail Newsletter Delivery
```

---

# 📌 Workflow Screenshot

![Personal AI & Tech News Email Generator using n8n](./assets/n8n%20workflow%20screenshot.png)

# 📷 Workflow Overview

The workflow automatically runs on a schedule, collects AI and tech updates from multiple sources, summarizes them using Gemini AI, and sends a personalized email newsletter.

---

# ⚙️ How This Automation Works

## 1️⃣ Schedule Trigger Starts the Workflow

The workflow starts automatically at a specific time every day using a `Schedule Trigger`.

Example:

```text
Every day at 8:00 AM
```

This allows fully automated daily newsletter generation.

---

## 2️⃣ RSS Feeds Fetch AI & Tech News

The workflow collects articles from multiple RSS feeds.

Example Sources:

- AI News Websites
- Tech Blogs
- Industry Updates
- Research Platforms

RSS feeds help gather recently published articles automatically.

---

## 3️⃣ SERP API Fetches Live AI Events

RSS feeds only provide published articles.

To fetch live information like:

- AI conferences
- Webinars
- Hackathons
- Events happening this week

the workflow uses `SERP API`.

SERP API searches Google in real-time and returns live search results from across the internet.

---

# 🌐 Understanding SERP API

`SERP API` allows applications to fetch Google search results through an API.

It helps retrieve:

- Real-time search results
- Event information
- Trending topics
- Current updates

Unlike RSS feeds, SERP API is not limited to a few subscribed websites.

---

# 🔗 Understanding the HTTP Request Node

The `HTTP Request` node is used to communicate with external APIs.

In this workflow:

```text
HTTP Request Node → Sends request
SERP API → Fetches Google search results
Response → Returns event data
```

The HTTP Request node acts as the bridge between n8n and external services.

---

## 4️⃣ Merge Node Combines All Data

The workflow merges:

- AI news articles
- Tech updates
- Live event information

into a single data stream.

This creates one centralized collection of information.

---

## 5️⃣ Aggregate Node Organizes Content

The aggregated content is cleaned and organized before sending it to Gemini AI.

This helps improve summary quality.

---

## 6️⃣ Google Gemini Summarizes Everything

The `Google Gemini Chat Model` analyzes all collected content and generates a concise newsletter summary.

Example:

```text
- Latest AI model releases
- Important tech updates
- Upcoming AI conferences
- Industry trends
```

This creates an easy-to-read personalized newsletter.

---

## 7️⃣ Gmail Sends the Newsletter

The final summarized newsletter is automatically delivered to the user's Gmail inbox.

The email contains:

- AI news summaries
- Tech updates
- Live event details
- Important highlights

---

# 🧩 Steps to Create This Automation

## Step 1 — Add Schedule Trigger

Add a `Schedule Trigger` node to run the workflow automatically.

Example:

```text
Daily at 8 AM
```

---

## Step 2 — Add RSS Feed Nodes

Add RSS feed nodes for:

- AI websites
- Technology blogs
- Research news

These nodes fetch the latest published articles.

---

## Step 3 — Add HTTP Request Node

Use an `HTTP Request` node to connect with SERP API.

This helps fetch real-time event information from Google search results.

---

## Step 4 — Configure SERP API Request

Inside the HTTP Request node:

- Add SERP API endpoint
- Add API key
- Add search query

Example Search:

```text
Upcoming AI events this week
```

---

## Step 5 — Merge All Data

Use a `Merge` node to combine:

- RSS feed data
- SERP API results

into one workflow stream.

---

## Step 6 — Aggregate Content

Use aggregation nodes to organize and prepare the collected information for summarization.

---

## Step 7 — Connect Google Gemini

Add the `Google Gemini Chat Model` node.

Provide prompts to summarize:

- AI news
- Tech updates
- Event information

into a clean newsletter format.

---

## Step 8 — Send Email Using Gmail

Add the Gmail node and configure:

- Recipient email
- Subject
- Newsletter content

The summarized newsletter will now be delivered automatically.

---

# ▶️ Running the Project

## Start Workflow

1. Open n8n
2. Execute the workflow
3. Keep workflow in `Active` state

---

## Automated Process

Once active, the workflow will:

- Fetch news automatically
- Search live events
- Generate summaries
- Send email newsletters daily

without manual work.

---

# 📚 What I Learned

Through this project, I learned:

- How RSS feeds work
- How APIs communicate with applications
- Using HTTP Request nodes inside n8n
- Fetching real-time data using SERP API
- AI-powered content summarization
- Building automated newsletter systems
- Integrating Gmail with automation workflows

---

# 🙌 Credits

Special thanks to NxtWave for teaching and guiding these AI automation concepts using n8n and AI tools.
