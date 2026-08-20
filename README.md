> **[中文](./README-CN.md)**
# 👋 Hi, I'm Martin 🌶️

📍 Chengdu, China | 💻 Java Infrastructure & Open Source Tool Builder

**13+ open-source projects · 2,000+ GitHub Stars in total**  
**5 projects officially featured  in [Awesome Java](https://github.com/akullpp/awesome-java)** (jquick-curl · jquick-pdf · jquick-java · jquick-excel · jquick-sql)  
**1,900+ commits in the past year** · Actively maintaining 15+ repositories

I build Java infrastructure, developer tools, and runtime systems — from language runtimes and query engines to network gateways and high-performance data processing.

I focus on building infrastructure that makes complex engineering tasks simpler, faster, and easier to integrate.

**Core methodology: declarative configuration-driven development** — you just "declare" what you want using XML or annotations, and the jquick toolchain automatically handles the rest of the complex execution logic.

**End-to-end infrastructure coverage**: from data collection (jquick-curl / jquick-connector), processing and aggregation (jquick-transform-function / jquick-java), persistence to database (jquick-datasource / jquick-mybatis), to final visualization (jquick-pdf / jquick-bi) — the entire process is seamlessly connected. Among them, **jquick-sql** serves as a **distributed federated virtual data warehouse engine**, providing a unified query entry for heterogeneous data sources at the upper layer and shielding underlying differences.

I believe in **"less is more"**: each tool solves exactly one problem, and solves it cleanly and thoroughly.

---

## JQuick Architecture

```text
                              JQuick
                                |
             +------------------+------------------+
             |                  |                  |
          Runtime              Data             Network
             |                  |                  |
     +-------+-------+    +-----+----------+       |
     |       |       |    |     |     |     |      |
 jquick-  jquick-  jquick- jquick- jquick- jquick- jquick-
 java     json     asm     sql    connector transform hub
                              |
                              |
                       Developer Tools
                              |
                +-------------+-------------+
                |             |             |
           jquick-curl   jquick-excel   jquick-pdf
```

## 📊 Open Source Commitment

| Metric | Data |
|--------|------|
| Total Stars | 2,000+ |
| Awesome Java inclusions | 5 projects |
| Actively maintained repos | 15+ |
| Commits in the past year | 1,900+ |

---

## 🧰 Core Domains & Tech Stack
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=flat-square&logo=node.js&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![npm](https://img.shields.io/badge/npm-CB3837?style=flat-square&logo=npm&logoColor=white)
![Apache Tomcat](https://img.shields.io/badge/Apache_Tomcat-F8DC75?style=flat-square&logo=apache-tomcat&logoColor=black)

---

## 🔌 Common Frameworks

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Spring Cloud](https://img.shields.io/badge/Spring_Cloud-6DB33F?style=flat-square&logo=spring&logoColor=white)
![MyBatis](https://img.shields.io/badge/MyBatis-EE3524?style=flat-square&logo=mybatis&logoColor=white)
![Pentaho](https://img.shields.io/badge/Pentaho-005C8A?style=flat-square&logo=pentaho&logoColor=white)
![Solr](https://img.shields.io/badge/Solr-D9411E?style=flat-square&logo=apache-solr&logoColor=white)
![ANTLR](https://img.shields.io/badge/ANTLR-4C7E9F?style=flat-square&logoColor=white)
![SVG](https://img.shields.io/badge/SVG-FFB13B?style=flat-square&logo=svg&logoColor=black)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vue.js&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white)
![PDF](https://img.shields.io/badge/PDF-FF0000?style=flat-square&logo=adobeacrobatreader&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=flat-square&logo=socket.io&logoColor=white)
![iText](https://img.shields.io/badge/iText-00A94F?style=flat-square&logo=itext&logoColor=white)

---

## 🌐 Contact Me

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=flat-square&logo=github&logoColor=white)](https://github.com/paohaijiao)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:goudingcheng@gmail.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=flat-square&logo=whatsapp&logoColor=white)](https://wa.me/601162366686)

---

## 📌 Current Projects

> 📦 All projects follow: **lightweight dependencies, low intrusion, out-of-the-box**

> **Note**: Projects marked with ✅ in the "XML Configuration Support" column refer to support for **declarative XML configuration files** similar to **MyBatis Mapper.xml** or **jquick-excel.xml** (i.e., defining mapping rules, styles, transformation logic, SQL bindings, and other business configurations via XML), rather than merely having basic XML parsing capabilities.

| Project | Description | Primary Use | XML Support? | Stars | Included in Awesome Java? |
|---------|-------------|-------------|--------------|-------|---------------------------|
| [jquick-hub](https://github.com/paohaijiao/jquick-hub) | jquick-hub (**TCP Gateway**) Available as a Docker image: docker pull **paohaijiao/jquick-hub:latest**| A high-performance protocol-sniffing **TCP gateway** built on Netty 4. It exposes a single public port and automatically routes inbound data package to different backends based on the first packet | ❌ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-hub?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-hub) | No |
| [jquick-json](https://github.com/paohaijiao/jquick-json) | using **JQuick-ASM** bytecode to generate alternative reflections, achieving a performance improvement of up to 54 times for JSON serialization/deserialization.| JQuick JSON is a bytecode-driven JSON serialization and deserialization library for Java. It leverages ASM to generate optimized object mapping code at runtime, reducing the overhead associated with reflection-based serialization. | ❌ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-json?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-json) | No |
| [jquick-curl](https://github.com/paohaijiao/jquick-curl) | Lightweight HTTP client — as concise as cURL, with uncompromising performance | **Curl as code**, replacement for OkHttp/Apache HttpClient | ✅ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-curl?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-curl) | Yes |
| [jquick-connector](https://github.com/paohaijiao/jquick-connector) | Universal data connector — converts any tool/data source into a unified in-memory data interface | **Unified access to heterogeneous data sources**, multi-source data adaptation | ✅ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-connector?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-connector) | No |
| [jquick-excel](https://github.com/paohaijiao/jquick-excel) | Zero-config Excel read/write tool — say goodbye to POI boilerplate, import/export in one line | High-performance Excel processing with **streaming**, style **caching**, **AST** caching, and shared **OPCPackage** parsing. | ✅ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-excel?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-excel) | Yes |
| [jquick-path](https://github.com/paohaijiao/jquick-path) | JSON Path query tool — concise syntax to quickly extract JSON data, like XPath for XML | Quickly extract values at specified paths from nested JSON | ❌ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-path?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-path) | No |
| [jquick-transform-function](https://github.com/paohaijiao/jquick-transform-function) | Universal data function library — provides 200+ out-of-the-box data processing methods | **SPI-based function** registry with support for dynamic extension | ✅ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-transform-function?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-transform-function) | No |
| [jquick-java](https://github.com/paohaijiao/jquick-java) | Dynamic business **scripting language** — combines Java's strong logic with XML declarative configuration | Dynamic business rule orchestration such as credit rating, risk scoring | ✅ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-java?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-java) | Yes |
| [jquick-pdf](https://github.com/paohaijiao/jquick-pdf) | Native Java PDF generation tool — **no browser/WebKit dependency**, built-in **30+ ECharts like chart types** | Server-side PDF report generation without a browser | ❌ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-pdf?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-pdf) | Yes |
| [jquick-mybatis](https://github.com/paohaijiao/jquick-mybatis) | Lightweight MyBatis enhancement framework — zero redundant annotations, zero business code intrusion | Simplifies MyBatis single-table CRUD, dynamic conditions, pagination, and multi-table associations | ✅ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-mybatis?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-mybatis) | No |
| [jquick-datasource](https://github.com/paohaijiao/jquick-datasource) | Universal data source management — supports automatic DDL/DML generation | Dynamically generate table creation / CRUD SQL, simplifying data source operations | ❌ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-datasource?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-datasource) | No |
| [jquick-sql](https://github.com/paohaijiao/jquick-sql) | Distributed **federated logical data warehouse** query SQL engine | Cross-database / cross-heterogeneous data source SQL federated analysis | ✅ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-sql?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-sql) | Yes |
| [jquick-bi](https://github.com/paohaijiao/jquick-bi) | Jquick-bi engine (Vue) | Online BI analytical processing (in development) | ✅ | [![Stars](https://img.shields.io/github/stars/paohaijiao/jquick-bi?style=flat-square&label=stars)](https://github.com/paohaijiao/jquick-bi) | No |

---

## 📊 GitHub Stats

- **1,580+** commits in the past year
- Actively maintaining **15+** Java open-source repositories
- Focus areas: lightweight tools, developer productivity, enterprise Java infrastructure

---

## 🧭 Philosophy

> **Simple, reliable, practical.**  
> The purpose of tools is to let developers forget about the tools themselves and focus on the real business logic.

I don't chase flashy tech. I pursue this — when you next face those "have-to-do-but-don't-want-to-spend-time-on" tasks like Excel, HTTP, or SQL, you'll remember "there's a tool that can handle it", and wrap it up within 5 minutes.

---

*Last updated: Spring 2026 · Continuously improving*
