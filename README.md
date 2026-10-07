<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:080808,45:111827,75:172554,100:0f3460&height=210&section=header&text=SOHAM%20PANWALKAR&fontSize=52&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=BACKEND%20%7C%20DISTRIBUTED%20SYSTEMS%20%7C%20AI%20AGENTS&descAlignY=62&descSize=15&descColor=3ff2e9" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono\&weight=600\&size=18\&duration=2800\&pause=1200\&color=3FF2E9\&center=true\&vCenter=true\&width=800\&lines=Backend+%2F+Distributed+Systems+%2F+AI+Agents;Building+Pulsar+%E2%80%94+autonomous+browser+automation;500%2B+LeetCode+problems+and+counting;Interested+in+systems+that+actually+ship.)](https://git.io/typing-svg)

<br>

[![GitHub](https://img.shields.io/badge/GitHub-notsamaltman-0d0d0d?style=for-the-badge\&logo=github\&logoColor=3ff2e9)](https://github.com/notsamaltman)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Soham%20Panwalkar-0d0d0d?style=for-the-badge\&logo=linkedin\&logoColor=3ff2e9)](https://www.linkedin.com/in/soham-panwalkar-ab672b351/)
[![Email](https://img.shields.io/badge/Email-panwalkarsoham%40gmail.com-0d0d0d?style=for-the-badge\&logo=gmail\&logoColor=e94560)](mailto:panwalkarsoham@gmail.com)

</div>

---

## About Me

<table width="100%">
<tr>
<td width="50%" valign="top">

```text
Name     : Soham Panwalkar
College  : DJSCE, Mumbai
Degree   : B.Tech Computer Engineering
Focus    : Backend / Systems / AI

Currently:
  - Building Pulsar
  - Grinding DSA
  - Learning system design
  - Building agent infrastructure
```

</td>

<td width="50%" valign="top">

I'm a Computer Engineering student interested in backend engineering, distributed systems and autonomous agents.

I enjoy building systems where the interesting problems are not just writing an API, but handling queues, workers, retries, state, failures, browser automation and real-time execution.

Currently spending most of my time building **Pulsar** and improving my DSA / backend fundamentals.

</td>
</tr>
</table>

---

## Tech Stack

<div align="center">

### Languages

<img src="https://skillicons.dev/icons?i=python,java,js,ts,c" />

<br><br>

### Backend

<img src="https://skillicons.dev/icons?i=nodejs,express,fastapi,flask,nextjs" />

<br><br>

### Databases & Infrastructure

<img src="https://skillicons.dev/icons?i=postgres,redis,docker,aws,supabase,cloudflare" />

<br><br>

### AI / Automation

<img src="https://skillicons.dev/icons?i=pytorch" />

<br>

<img src="https://img.shields.io/badge/LangGraph-0d0d0d?style=for-the-badge&logoColor=3ff2e9"/>
<img src="https://img.shields.io/badge/LangChain-0d0d0d?style=for-the-badge&logoColor=3ff2e9"/>
<img src="https://img.shields.io/badge/Playwright-0d0d0d?style=for-the-badge&logo=playwright&logoColor=2EAD33"/>
<img src="https://img.shields.io/badge/BullMQ-0d0d0d?style=for-the-badge&logoColor=e94560"/>
<img src="https://img.shields.io/badge/Ollama-0d0d0d?style=for-the-badge&logoColor=ffffff"/>
<img src="https://img.shields.io/badge/Groq-0d0d0d?style=for-the-badge&logoColor=ffffff"/>

<br><br>

### Tools

<img src="https://skillicons.dev/icons?i=git,github,githubactions,linux,postman,vscode" />

</div>

---

## LeetCode

<div align="center">

[![LeetCode](https://img.shields.io/badge/LeetCode-500%2B%20Problems-FFA116?style=for-the-badge\&logo=leetcode\&logoColor=white)](https://leetcode.com/)
[![DSA](https://img.shields.io/badge/Focus-DSA-3ff2e9?style=for-the-badge)](https://leetcode.com/)

</div>

```text
500+ problems solved

Current focus:
  Trees       Graphs       Dynamic Programming
  DSU / MST   Tries        Binary Search
  BFS / DFS   Bit Tricks   Interview Patterns
```

I don't really care about the number by itself. The main goal has been getting better at recognizing patterns and being able to derive a solution instead of memorizing one.

---

# Projects

<table width="100%">
<tr>

<td width="50%" valign="top">

## Pulsar

### Autonomous Lead Generation Platform

Pulsar is the main project I'm currently building.

It uses LLM agents, browser automation and distributed workers to automate lead generation and outreach workflows.

```text
Frontend
  Next.js + Supabase

Agent Service
  FastAPI
  LangGraph
  Groq / VLMs

Workers
  BullMQ
  Redis

Browser
  Playwright

Communication
  SSE
```

Some of the things I've been working on:

* Hierarchical agent orchestration
* ICP generation and task delegation
* Browser-based lead discovery
* DOM + screenshot based actions
* VLM-driven browser interaction
* Async job execution with BullMQ
* Redis-backed job state
* Retries and execution recovery
* Real-time progress through SSE
* Job queue / ETA estimation
* Model rate-limit and quota handling
* Worker health heartbeats
* Daily usage limits

Current benchmark:

```text
100 leads
~20 minutes
~80% worth reviewing
```

</td>

<td width="50%" valign="top">

## RepoGenie

### Repository Understanding System

A tool for analysing large GitHub repositories without requiring the entire repository to be cloned locally.

```text
FastAPI
   +
LangGraph
   +
Vector Search
   +
Next.js
```

The goal is to turn an unfamiliar codebase into something that is easier to understand and navigate.

The system can work with repository structure and source files to extract useful architectural information and relationships between components.

```text
GitHub Repository
       |
       v
Repository Structure
       |
       v
Code Analysis
       |
       v
Embeddings / Retrieval
       |
       v
LLM Reasoning
       |
       v
Architectural Insights
```

</td>

</tr>
</table>

---

## Pulsar Architecture

```text
                         User
                           |
                           v
                  +----------------+
                  |    Next.js     |
                  |    Frontend    |
                  +-------+--------+
                          |
                          v
                  +----------------+
                  |   Master Agent |
                  |    LangGraph   |
                  +-------+--------+
                          |
             +------------+------------+
             |            |            |
             v            v            v
        Agent A       Agent B      Agent C
             |            |            |
             +------------+------------+
                          |
                          v
                  +----------------+
                  | Redis / BullMQ |
                  |                |
                  | Jobs           |
                  | Retries        |
                  | Worker state   |
                  +-------+--------+
                          |
                          v
                  +----------------+
                  |   ML Service   |
                  |    FastAPI     |
                  +-------+--------+
                          |
                          v
                  +----------------+
                  |   Playwright   |
                  |    Browser     |
                  +-------+--------+
                          |
                          v
                   External Sites
```

One of the problems I'm particularly interested in is making browser agents reliable.

A model producing the right action once is easy.

Getting an agent to deal with:

```text
wrong element
     |
page changed
     |
action failed
     |
retry
     |
model temporarily rate limited
     |
resume
     |
browser restriction
     |
recover
```

is much closer to the actual engineering problem.

---

# Experience

```text
2026 — PRESENT
DeepCytes Cyber Labs UK
Full Stack / Backend Developer Intern

  • Improved API response times by ~15% using Redis caching
    and database lookup optimization

  • Built backend routes for cybersecurity workflows
    involving CVE data and security agents

  • Worked on authenticated API workflows and backend
    infrastructure


JAN 2026 — APR 2026
Shresht / Sugamaya Governance
Full Stack Developer Intern

  • Built and deployed 8+ client-facing web platforms

  • Developed registration systems and analytics dashboards

  • Worked with Next.js, Supabase and backend integrations

  • Worked on asynchronous publishing and interaction
    workflows for a video platform
```

---

# GitHub

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=notsamaltman&show_icons=true&theme=transparent&hide_border=true&title_color=3ff2e9&icon_color=3ff2e9&text_color=a0a0b0&bg_color=0d0d0d&ring_color=3ff2e9&include_all_commits=true&count_private=true" height="180"/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=notsamaltman&theme=transparent&hide_border=true&ring=3ff2e9&fire=e94560&currStreakLabel=3ff2e9&sideLabels=a0a0b0&dates=a0a0b0&currStreakNum=ffffff&sideNums=ffffff&background=0d0d0d&stroke=1a1a2e" height="180"/>

</div>

<br>

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=notsamaltman&theme=github-compact&hide_border=true&bg_color=0d0d0d&color=a0a0b0&line=3ff2e9&point=ffffff&area=true" width="100%"/>

</div>

---

# GitHub Trophies

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=notsamaltman&column=7&margin-w=15&margin-h=15&no-bg=true&no-frame=true&theme=darkhub" width="90%"/>

</div>

---

# Contribution Graph

<div align="center">

<img src="https://raw.githubusercontent.com/notsamaltman/notsamaltman/output/github-contribution-grid-snake.svg" width="100%"/>

</div>

---

## Currently Working On

<table width="100%">
<tr>
<td width="50%" valign="top">

### Pulsar

* More reliable browser agents
* Better action execution
* Lower inference costs
* Queue management
* Worker health monitoring
* Better failure recovery
* Production deployment

</td>

<td width="50%" valign="top">

### Personal

* 500+ → 1000 LeetCode
* System design
* Backend architecture
* Distributed systems
* Competitive programming
* Building and shipping more

</td>
</tr>
</table>

---

<div align="center">

[![Email](https://img.shields.io/badge/panwalkarsoham%40gmail.com-0d0d0d?style=for-the-badge\&logo=gmail\&logoColor=e94560)](mailto:panwalkarsoham@gmail.com)
  
[![GitHub](https://img.shields.io/badge/notsamaltman-0d0d0d?style=for-the-badge\&logo=github\&logoColor=a0a0b0)](https://github.com/notsamaltman)
  
[![LinkedIn](https://img.shields.io/badge/sohampanwalkar-0d0d0d?style=for-the-badge\&logo=linkedin\&logoColor=a0a0b0)](https://www.linkedin.com/in/soham-panwalkar-ab672b351/)

<br><br>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f3460,50:111827,100:080808&height=120&section=footer&reversal=true" width="100%"/>

</div>
