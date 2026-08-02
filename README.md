<h1 align="center">
  <strong>I'm Aaditya Sinha</strong>
</h1>

I am a GenAI Analyst at OakNorth Bank and a forward deployed engineer embedded in People Operations, where I
build organisation wide internal tools, agentic AI workflows and the cloud infrastructure that runs underneath
them. Outside work I build quantitative trading tooling from first principles and play a reasonable game of chess.

<p align="center">
  <a href="https://www.linkedin.com/in/555aaditya/"><strong>&#8598; linkedin</strong></a> &nbsp;
  <a href="https://github.com/aaditya-sinha-oaknorth"><strong>&#8598; oaknorth</strong></a> &nbsp;
  <a href="#selected-projects" title="projects listed below"><strong>&#8601; projects</strong></a> &nbsp;
  <a href="https://leetcode.com/555aaditya/"><strong>&#8598; leetcode</strong></a> &nbsp;
  <a href="https://www.kaggle.com/aaditya555"><strong>&#8598; kaggle</strong></a> &nbsp;
  <a href="https://www.chess.com/member/555aaditya"><strong>&#8598; chess</strong></a> &nbsp;
  <a href="mailto:555aaditya@proton.me"><strong>&#8598; mail</strong></a> &nbsp;
</p>

### Currently @ OakNorth

I own an internal tools platform and the people product built on top of it end to end, from the React frontend
through the Python services down to the Terraform that provisions all of it.

- I design and deploy **agentic AI workflows and subagents** with Claude, covering multi agent orchestration and event driven automation through Power Automate, all sitting behind an audited LLM layer that masks PII and falls back deterministically when no key is available.
- The **internal tooling platform** is a launcher SPA with a build time validated tool registry and code split mounting, so a new organisation wide tool ships a registry entry instead of standing up its own auth, CDN and gateway.
- The **frontend** is React 19 and TypeScript 5.9 on Vite 6 with React Router 7 and a strict in house design system, and the role resolved for each user drives every screen and navigation path they see.
- The **backend** is FastAPI with SQLAlchemy 2.0, Alembic and Pydantic v2 on Python 3.13, covering a cycle state machine, a rating engine, calibration, 360 feedback and an idempotent event keyed notification system.
- Every layer of the **delivery path** is provisioned in Terraform and runs from CloudFront and WAF through a Lambda proxy signed with OAC SigV4 into a private API Gateway with its own JWT authoriser, then over a VPC Link to an internal NLB, ECS Fargate and Aurora Serverless v2.
- I contribute reusable modules back to the bank's **shared Terraform library**, including per origin CloudFront OAC and WAF request size exceptions, and I look after network address pools and container registries alongside them.
- **GitHub Actions** pipelines run test, build, migration and deploy across every service.
- **Auth0 federated to Microsoft Entra ID** handles identity, with custom post login Actions mapping SSO groups to permission claims that are enforced at the gateway authoriser and checked again in the backend against field level capability rules.
- An **HRIS sync** keeps the org chart current and feeds workforce reporting, people insights and the live dashboards built on top of it.

### Selected Projects

<div align="center">

|                        Project | Description                                                                                      |
| -----------------------------: | :------------------------------------------------------------------------------------------------ |
|          **Quant & Trading**   |                                                                                                  |
|  [Stock-Backtesting-Pipeline]  | Algorithmic backtesting engine built from mathematical first principles with no pandas or numpy. |
|          [StockMarketAnalysis] | Dockerised Kafka producer streaming live market data.                                            |
|         **Backend & APIs**     |                                                                                                  |
|    [Optimised-Fuel-Route-API]  | Finds the cheapest fuel stops on any US route with a grid spatial index and greedy DP.           |
|                      [JamRoom] | Real time collaborative music player built on Flask, Socket.IO and the Spotify Web API.          |
|                [URL-Shortener] | Link shortener with fast redirects and analytics tracking.                                       |
|                     [Eventora] | MERN event ticketing app with auth, calendar views and payment summaries.                        |
|       **Data Engineering**     |                                                                                                  |
|                 [Apache-Kafka] | Producers, consumers and topic operations built up from the ground.                              |
|     [SalesPerformanceDashboard] | Exploratory sales analysis and KPI reporting in Jupyter.                                         |
|   **ML, LLM and Computer Vision** |                                                                                                  |
|               [Gaze-Detection] | Exam proctoring using 68 point facial landmarks and YOLO phone detection.                        |
|              [Language-Model] | From-scratch GPT-style language model: byte-level BPE, GQA + RoPE, tiled flash attention, hand-written AdamW, cached inference & benchmarking. |
|      **Learning & Reference**  |                                                                                                  |
|      [Competitive-Programming] | NeetCode and Codeforces solutions.                                                               |
| [data-structures-and-algorithms] | DSA implementations and notebooks.                                                               |
|                        [Books] | Systems, compilers and architecture reading list.                                                |

</div>

[Apache-Kafka]: https://github.com/555aaditya/Apache-Kafka
[Books]: https://github.com/555aaditya/Books
[Competitive-Programming]: https://github.com/555aaditya/Competitive-Programming
[data-structures-and-algorithms]: https://github.com/555aaditya/data-structures-and-algorithms
[Eventora]: https://github.com/555aaditya/Eventora
[Gaze-Detection]: https://github.com/555aaditya/Gaze-Detection
[JamRoom]: https://github.com/555aaditya/JamRoom
[Language-Model]: https://github.com/555aaditya/Language-Model
[Optimised-Fuel-Route-API]: https://github.com/555aaditya/Optimised-Fuel-Route-API
[SalesPerformanceDashboard]: https://github.com/555aaditya/SalesPerformanceDashboard
[Stock-Backtesting-Pipeline]: https://github.com/555aaditya/Stock-Backtesting-Pipeline
[StockMarketAnalysis]: https://github.com/555aaditya/StockMarketAnalysis
[URL-Shortener]: https://github.com/555aaditya/URL-Shortener

### Technologies I have worked with

<div align="center">

|                     Domain | Stack                                                                                            |
| -------------------------: | :--------------------------------------------------------------------------------------------------- |
|              **Languages** | Python · TypeScript · C++ · SQL · Bash                                                              |
|        **AI & Automation** | Claude · Agentic workflows · Subagents · Multi agent orchestration · Power Automate                 |
|                **Backend** | FastAPI · SQLAlchemy · Alembic · Pydantic · Flask · Django · REST                                   |
|               **Frontend** | React · TypeScript · Vite · React Router · styled components                                        |
| **Cloud & Infrastructure** | AWS ECS Fargate · Lambda · API Gateway · CloudFront · WAF · S3 · EC2 · Terraform · Docker           |
|        **CI/CD & Tooling** | GitHub Actions · Poetry · pytest · Git                                                              |
|      **Identity & Access** | Auth0 · Microsoft Entra ID · OIDC/PKCE · JWT · RBAC                                                 |
|              **Databases** | PostgreSQL · Aurora · MongoDB · Redis · SQLite                                                      |
|       **Data Engineering** | Airflow · Kafka · Pandas · ETL pipelines                                                            |
|         **Analytics & BI** | Power BI · Tableau · Plotly · Matplotlib · Seaborn                                                  |
|        **Quant & Finance** | Backtesting engines · Black model options pricing · Greeks · Walk forward validation                |
|   **ML & Computer Vision** | OpenCV · YOLO · dlib · scikit-learn · TensorFlow                                                    |

</div>

### LeetCode

<p align="center">
  <img src="https://leetcard.jacoblin.cool/555aaditya?ext=heatmap">
</p>

<p align="center">
  <a href="https://www.chess.com/member/555aaditya">chess.com</a>
  <img align="center" src="https://img.shields.io/badge/dynamic/json?logo=chessdotcom&label=rapid&query=%24.chess_rapid.last.rating&url=https%3A%2F%2Fapi.chess.com%2Fpub%2Fplayer%2F555aaditya%2Fstats">
</p>
