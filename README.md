<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2563EB,100:06B6D4&height=180&section=header&text=Ke%20Zhang&fontSize=48&fontColor=ffffff&fontAlignY=42&animation=fadeIn" alt="Ke Zhang" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1200&color=2563EB&center=true&vCenter=true&width=560&lines=Backend+Developer;AI+Agent+Developer;Building+with+.NET+%26+LLMs" alt="Backend Developer · AI Agent Developer · Building with .NET & LLMs" />

📍 Christchurch, New Zealand

[![Open Work Rights – NZ](https://img.shields.io/badge/Open_Work_Rights-New_Zealand-2563EB?style=flat-square)](#)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-2563EB?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kezhang/)
[![Email](https://img.shields.io/badge/Email-06B6D4?style=flat-square&logo=gmail&logoColor=white)](mailto:kzhangdevnz@gmail.com)

</div>

<br/>

### About

I'm a software developer focused on **backend and AI agent development** — turning user and
business needs into working systems with C#/.NET, APIs, databases, cloud services, and LLMs,
including designing and building LLM-driven agent workflows end to end. I like taking
ownership of a problem, working independently, and staying close to stakeholders while I build it.

*Also trained in visual design before moving into software — which is part of why this README isn't plain text.*

<br/>

### 🔭 Currently

- 🤖 Building **[KONER Agent](https://green-meadow07a664610.3.azurestaticapps.net/)** — an LLM tool-calling agent that analyses time records and proposes schedule changes
- 🚀 Full-stack developer at **Microsoft Student Accelerator (MSA) 2026**, Auckland — shipping **[Footprint v2](https://footprint-v2-client.onrender.com/)**

<br/>

### 🧰 Tech Stack

<table>
<tr><td><b>Backend</b></td><td>
<img src="https://skillicons.dev/icons?i=cs,dotnet" height="32" alt="C#, .NET"/>
<img src="https://img.shields.io/badge/EF_Core-2563EB?style=flat-square" alt="EF Core"/>
<img src="https://img.shields.io/badge/REST_APIs-2563EB?style=flat-square" alt="REST APIs"/>
<img src="https://img.shields.io/badge/SQL-2563EB?style=flat-square" alt="SQL"/>
<img src="https://img.shields.io/badge/JWT-2563EB?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT"/>
</td></tr>
<tr><td><b>AI Engineering</b></td><td>
<img src="https://img.shields.io/badge/LLM_Integration-06B6D4?style=flat-square" alt="LLM Integration"/>
<img src="https://img.shields.io/badge/AI_Agents-06B6D4?style=flat-square" alt="AI Agents"/>
<img src="https://img.shields.io/badge/Tool_Calling-06B6D4?style=flat-square" alt="Tool Calling"/>
<img src="https://img.shields.io/badge/RAG-06B6D4?style=flat-square" alt="RAG"/>
<img src="https://img.shields.io/badge/Gemini_API-06B6D4?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini API"/>
<img src="https://img.shields.io/badge/Azure_OpenAI-06B6D4?style=flat-square&logo=microsoftazure&logoColor=white" alt="Azure OpenAI"/>
</td></tr>
<tr><td><b>Data</b></td><td>
<img src="https://skillicons.dev/icons?i=postgres,mysql,sqlite" height="32" alt="PostgreSQL, MySQL, SQLite"/>
</td></tr>
<tr><td><b>Frontend</b></td><td>
<img src="https://skillicons.dev/icons?i=react,ts,nextjs,tailwind" height="32" alt="React, TypeScript, Next.js, Tailwind CSS"/>
</td></tr>
<tr><td><b>Cloud &amp; DevOps</b></td><td>
<img src="https://skillicons.dev/icons?i=azure,docker,githubactions" height="32" alt="Azure, Docker, GitHub Actions"/>
</td></tr>
<tr><td><b>Tools</b></td><td>
<img src="https://skillicons.dev/icons?i=git,github,postman,linux" height="32" alt="Git, GitHub, Postman, Linux"/>
<img src="https://img.shields.io/badge/Swagger-2563EB?style=flat-square&logo=swagger&logoColor=white" alt="Swagger"/>
<img src="https://img.shields.io/badge/Claude_Code-2563EB?style=flat-square" alt="Claude Code"/>
<img src="https://img.shields.io/badge/Cursor-2563EB?style=flat-square" alt="Cursor"/>
<img src="https://img.shields.io/badge/GitHub_Copilot-2563EB?style=flat-square" alt="GitHub Copilot"/>
</td></tr>
<tr><td><b>Methodologies</b></td><td>
<img src="https://img.shields.io/badge/Agile-06B6D4?style=flat-square" alt="Agile"/>
<img src="https://img.shields.io/badge/Scrum-06B6D4?style=flat-square" alt="Scrum"/>
<img src="https://img.shields.io/badge/Jira-06B6D4?style=flat-square&logo=jira&logoColor=white" alt="Jira"/>
</td></tr>
</table>

<br/>

### 💡 Featured Projects

#### 🤖 KONER Agent — *Jul 2026 – Present*

An AI-powered time-management agent that uses **LLM-driven tool calling** to analyse a user's
time records, hold conversational context, and propose schedule changes that require the
user's approval before anything actually changes.

- Built the ASP.NET Core Web API and agent service, including the AI analysis endpoint that
  orchestrates LLM-driven analysis for the React frontend
- Integrated the Google Gemini API and implemented the **agent loop** — tool selection,
  execution, result processing, and context-aware response generation
- Designed reusable agent tools wired to **PostgreSQL via EF Core** for user-specific time-record retrieval
- Implemented **persistent user memory** and conversation history for continuity across sessions
- Containerised with Docker; GitHub Actions CI/CD deploys automatically to Azure on push

```mermaid
flowchart LR
    U[React Frontend] -->|user query| A[ASP.NET Core API]
    A --> L{Agent Loop}
    L -->|selects & runs| T[Agent Tools]
    T --> D[(PostgreSQL via EF Core)]
    D --> L
    L -->|context-aware response| U
    M[(Persistent Memory & History)] <--> L
```

<img src="https://img.shields.io/badge/ASP.NET_Core-2563EB?style=flat-square" alt="ASP.NET Core"/> <img src="https://img.shields.io/badge/Gemini_API-2563EB?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini API"/> <img src="https://img.shields.io/badge/PostgreSQL-2563EB?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/> <img src="https://img.shields.io/badge/Docker-2563EB?style=flat-square&logo=docker&logoColor=white" alt="Docker"/> <img src="https://img.shields.io/badge/GitHub_Actions-2563EB?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
&nbsp;→&nbsp; [**Live demo**](https://green-meadow07a664610.3.azurestaticapps.net/)

<br/>

<table>
<tr>
<td width="50%" valign="top">

**🌍 Footprint v2** — *Feb 2026 – Present*

Online travel community platform built during the Microsoft Student Accelerator 2026
internship — RESTful APIs, JWT authentication, RBAC, post sharing, city collections, and
gamification (points, leaderboards, achievement badges).

<img src="https://img.shields.io/badge/ASP.NET_Core-2563EB?style=flat-square" alt="ASP.NET Core"/> <img src="https://img.shields.io/badge/EF_Core-2563EB?style=flat-square" alt="EF Core"/> <img src="https://img.shields.io/badge/React-2563EB?style=flat-square&logo=react&logoColor=white" alt="React"/> <img src="https://img.shields.io/badge/TypeScript-2563EB?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>

[**Live demo →**](https://footprint-v2-client.onrender.com/)

</td>
<td width="50%" valign="top">

**💼 Wingman Ltd** — *Jun 2025 – Nov 2025 (internship)*

Genetics data platform for dairy decision-making. Synced 20,000+ bull records from external
sources and shipped favourites, genetic-parameter comparison, and an email-based consultation
workflow.

<img src="https://img.shields.io/badge/C%23-06B6D4?style=flat-square" alt="C#"/> <img src="https://img.shields.io/badge/.NET-06B6D4?style=flat-square" alt=".NET"/> <img src="https://img.shields.io/badge/SQL-06B6D4?style=flat-square" alt="SQL"/> <img src="https://img.shields.io/badge/Git-06B6D4?style=flat-square&logo=git&logoColor=white" alt="Git"/>

Achievement: delivered the Phase 1 MVP — 6 independently built features

</td>
</tr>
</table>

<br/>

### 📊 GitHub Activity

<div align="center">

<img src="https://github-stats-extended.vercel.app/api?username=KeZhang-dev&show_icons=true&theme=default&hide_border=true&title_color=2563EB&icon_color=06B6D4&text_color=333333" alt="Ke Zhang's GitHub Stats" height="165"/>
<img src="https://github-stats-extended.vercel.app/api/top-langs/?username=KeZhang-dev&layout=compact&hide_border=true&title_color=2563EB&text_color=333333" alt="Top Languages" height="165"/>

<img src="https://streak-stats.demolab.com/?user=KeZhang-dev&hide_border=true&stroke=2563EB&ring=06B6D4&fire=06B6D4&currStreakLabel=2563EB" alt="GitHub Streak Stats"/>

</div>

<br/>

### 🎓 Certifications &amp; Education

<img src="https://img.shields.io/badge/AZ--900-Azure_Fundamentals-2563EB?style=flat-square&logo=microsoftazure&logoColor=white" alt="AZ-900 Azure Fundamentals"/>
<img src="https://img.shields.io/badge/AI--900-Azure_AI_Fundamentals-2563EB?style=flat-square&logo=microsoftazure&logoColor=white" alt="AI-900 Azure AI Fundamentals"/>
<img src="https://img.shields.io/badge/CLF--C02-AWS_Cloud_Practitioner-06B6D4?style=flat-square&logo=amazonaws&logoColor=white" alt="CLF-C02 AWS Certified Cloud Practitioner"/>

Master of Applied Computing — Lincoln University, New Zealand (2024–2025)

<br/>

---

<div align="center">

📫 **kzhangdevnz@gmail.com** &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/kezhang/) &nbsp;·&nbsp; Open to backend / AI agent developer roles in New Zealand

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2563EB,100:06B6D4&height=100&section=footer" alt="" width="100%"/>

</div>
