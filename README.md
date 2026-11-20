<div align="center">

<img src="./assets/hero-control-deck.svg" width="100%" alt="Ayman Ali — Cyber-Industrial AI Control Deck" />

<br/>

<p align="center">
  <a href="mailto:ayman.m.ali148@gmail.com">
    <img src="https://img.shields.io/badge/TRANSMIT_EMAIL-ayman.m.ali148%40gmail.com-0EA5E9?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0B1324" alt="Email" />
  </a>
  <a href="https://github.com/aymanmali">
    <img src="https://img.shields.io/badge/GITHUB_CONSOLE-@aymanmali-10B981?style=for-the-badge&logo=github&logoColor=white&labelColor=0B1324" alt="GitHub" />
  </a>
  <img src="https://img.shields.io/badge/BASE-MUNICH,_GERMANY_🇩🇪-F59E0B?style=for-the-badge&labelColor=0B1324" alt="Munich, Germany" />
</p>

</div>

---

<div align="center">
  <img src="./assets/bento-telemetry.svg" width="100%" alt="Core Engineering Capabilities Bento Grid" />
</div>

<details>
<summary><b>🛰️ Inspect Full System Architecture &amp; Technical Matrix (Click to Expand)</b></summary>
<br/>

```mermaid
flowchart LR
    subgraph EDGE["01 // Physical & Edge Layer"]
        HW["ESP32 C (ESP-IDF)\nKiCad Custom PCB"]
        BUS["RS-485 CRC-16\nMQTT / RTSP Ingest"]
        HW --- BUS
    end

    subgraph VISION["02 // Machine Vision Engine"]
        DET["YOLOv8 / ONNX Runtime\nPyTorch CNN Classifier"]
        ROI["OpenCV ROI Polygons\nIoU Tracking & OCR"]
        DET --> ROI
    end

    subgraph AGENT["03 // Agentic AI & MCP Core"]
        GRAPH["LangGraph / LangChain\nStateful Orchestration"]
        MCP["FastMCP / MCP Servers\nDynamic Tool Calling"]
        GRAPH <--> MCP
    end

    subgraph CLOUD["04 // Cloud & BI Runtime"]
        API["FastAPI REST + WebSockets\nDocker & GCP Linux"]
        DATA["DuckDB-Wasm • PostgreSQL\nApache ECharts • Next.js"]
        API --> DATA
    end

    EDGE ==> VISION ==> AGENT ==> CLOUD
```

| 💻 Core Programming & APIs | 🧠 Machine Learning & Vision | 🤖 Agentic AI & LLM Systems | ☁️ Cloud, Data & DevOps |
| :--- | :--- | :--- | :--- |
| • Python & TypeScript | • PyTorch & Scikit-learn | • LangGraph & LangChain | • Docker & Docker Compose |
| • FastAPI (REST & WebSockets) | • YOLOv8 & ONNX Runtime | • Model Context Protocol (MCP) | • Google Cloud Platform (GCP) |
| • Embedded C (`ESP-IDF`) | • OpenCV ROI & Multi-Frame OCR | • Dynamic Tool Calling | • Linux & GitHub Actions CI/CD |
| • SQL, PostgreSQL & SQLite WAL | • Temporal Hysteresis & Tracking | • Structured Prompt Engineering | • DuckDB-Wasm & Apache ECharts |
| • RS-485 (`CRC-16`) & MQTT | • In-RAM Privacy Redaction | • Automated Model Evaluation | • KiCad PCB Design |

</details>

<br/>

<div align="center">
  <img src="./assets/section-projects.svg" width="100%" alt="01 — Featured Engineering Systems" />
</div>

<table>
  <tr>
    <td width="50%" valign="top">
      <code>SYS-01 // EDGE VISION • EMBEDDED • FASTAPI</code>
      <h3>🅿️ <a href="https://github.com/aymanmali/smart-parking-guidance-system">Smart Parking Guidance &amp; Management System</a></h3>
      <p>End-to-end automated computer-vision parking guidance platform for a <b>300-slot facility</b> (4 zones × 75 slots, 12 edge cameras, 2 entrance counters, 4 intersection directional screens), inspired by my 2019 field deployment at <b>Galleria40 Mall (LEED-certified)</b>.</p>
      <ul>
        <li><b>Edge Vision Pipeline:</b> YOLOv8 vehicle detection in PyTorch paired with calibrated per-slot OpenCV ROI polygons, a lightweight PyTorch CNN classifier, and temporal hysteresis filtering.</li>
        <li><b>Real-Time Guidance Backend:</b> FastAPI REST + WebSocket routing engine with an MQTT &amp; RS-485/CRC-16 hardware protocol bridge.</li>
        <li><b>Signage UI &amp; Custom Hardware:</b> React operator dashboard &amp; live LED signage simulator, plus ESP32 Embedded C (ESP-IDF) firmware and a custom KiCad PCB (<code>SPG-CTRL-v1</code>).</li>
      </ul>
      <details>
        <summary><b>⚙️ System Telemetry &amp; Hardware Specs</b></summary>
        <ul>
          <li><b>Field Pedigree:</b> Architected &amp; deployed in 2019 at Galleria40 (Sheikh Zayed, Egypt) to cut stall-search cruising and garage exhaust load.</li>
          <li><b>Wire Protocol:</b> Bit-accurate MODBUS/CRC-16 RS-485 binary framing with 15-second amber offline hardware failover and C99 unit tests.</li>
        </ul>
      </details>
      <br/>
      <a href="https://smart-parking-guidance-system.vercel.app"><img src="https://img.shields.io/badge/▶_LAUNCH_LIVE_SIMULATOR-10B981?style=flat-square&logo=vercel&logoColor=white" alt="Live Demo"/></a>
      <a href="https://github.com/aymanmali/smart-parking-guidance-system"><img src="https://img.shields.io/badge/SOURCE-181717?style=flat-square&logo=github&logoColor=white" alt="Source"/></a>
      <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch"/>
      <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="OpenCV"/>
      <img src="https://img.shields.io/badge/YOLOv8-111F68?style=flat-square" alt="YOLOv8"/>
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>
      <img src="https://img.shields.io/badge/ESP32_C-E7352C?style=flat-square&logo=espressif&logoColor=white" alt="ESP32"/>
    </td>
    <td width="50%" valign="top">
      <code>SYS-02 // IN-BROWSER OLAP • BI • AST COMPILER</code>
      <h3>🦆 <a href="https://github.com/aymanmali/quackboard">QuackBoard: Open-Source BI &amp; Analytics Platform</a></h3>
      <p>Open-source, Tableau-style Business Intelligence web platform powered by <b>DuckDB-Wasm</b>, <b>Apache ECharts</b>, and <b>Next.js 15</b> for zero-setup browser file analytics and live SQL dashboards.</p>
      <ul>
        <li><b>Hybrid Query Engine:</b> In-browser DuckDB-Wasm Web Worker SQL over CSV/Parquet/Excel/JSON files plus live PostgreSQL &amp; MySQL connections with AES-256-GCM encrypted credentials.</li>
        <li><b>Tableau-Style Chart Studio:</b> Drag-and-drop Dimension &amp; Measure shelves with 9 interactive chart types, date bucketing, and a read-only ad-hoc SQL Lab.</li>
        <li><b>Interactive Dashboards:</b> Drag-and-resize grid layouts, global filters, click-to-cross-filter across sibling charts, PNG/CSV export, and portable <code>.quackboard.json</code> import/export.</li>
      </ul>
      <details>
        <summary><b>⚙️ Query Compiler &amp; Security Specs</b></summary>
        <ul>
          <li><b>Visual AST Compiler:</b> Compiles shelf pills into parameterized, dialect-aware SQL (DuckDB / PostgreSQL / MySQL) with zero raw string interpolation.</li>
          <li><b>Read-Only Guardrails:</b> Single-pass SQL comment/literal scanner restricting ad-hoc queries to <code>SELECT</code>/<code>WITH</code> inside read-only transactions with query timeouts.</li>
        </ul>
      </details>
      <br/>
      <a href="https://quackboard-rosy.vercel.app"><img src="https://img.shields.io/badge/▶_LAUNCH_LIVE_BI_STUDIO-38BDF8?style=flat-square&logo=vercel&logoColor=black" alt="Live Demo"/></a>
      <a href="https://github.com/aymanmali/quackboard"><img src="https://img.shields.io/badge/SOURCE-181717?style=flat-square&logo=github&logoColor=white" alt="Source"/></a>
      <img src="https://img.shields.io/badge/DuckDB--Wasm-F59E0B?style=flat-square&logo=duckdb&logoColor=black" alt="DuckDB-Wasm"/>
      <img src="https://img.shields.io/badge/Next.js_15-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
      <img src="https://img.shields.io/badge/Apache_ECharts-AA344D?style=flat-square&logo=apacheecharts&logoColor=white" alt="Apache ECharts"/>
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
    </td>
  </tr>
  <tr>
    <td colspan="2" valign="top">
      <code>SYS-03 // EDGE AI DAEMON • DSGVO PRIVACY-BY-DESIGN • BILINGUAL PORTALS (DE/EN)</code>
      <h3>🚘 <a href="https://github.com/aymanmali/parkvektor-private-de">ParkVektor Private DE: Barrierless ANPR Parking Platform</a></h3>
      <p>An independent barrier-free ANPR private parking &amp; ticketing MVP designed for <b>Germany</b> (malls, retail parks, hotels, hospitals) around <b>DSGVO Privacy-by-Design</b> principles and German civil/tax workflows (<code>BGB</code>, <code>§ 147 AO</code>, <code>§ 39 StVG</code>).</p>
      <ul>
        <li><b>Hybrid Edge AI &amp; Smart ANPR:</b> Standalone Python Edge AI daemon (RTSP/ONVIF ingest, ONNX Runtime YOLO vehicle/plate detection, EU/DE slot+CTC plate OCR with IoU multi-frame voting, German <code>FE-Schrift</code> normalization, in-RAM face/windshield blurring, SQLite WAL offline sync) plus signed webhook adapters for commercial ANPR cameras (Axis, Adaptive Recognition, Hikvision, Generic JSON).</li>
        <li><b>Tariffs, Payments &amp; DSGVO Auto-Purge:</b> Flexible weekday/weekend tariffs, pluggable Stripe checkout (SEPA, Apple Pay, Google Pay, PayPal) with <code>19% MwSt.</code> PDF invoices, and automated raw-plate/snapshot purging with zero-PII audit logs.</li>
        <li><b>Bilingual Portals (DE/EN):</b> Next.js Driver QR Pay &amp; AutoPay wallets, German QWERTZ Pay-on-Foot Kiosk, Tenant Validation, Driver <i>Widerspruchsportal</i>, and Operator Admin / <code>§ 39 StVG</code> QA dashboard.</li>
      </ul>
      <details>
        <summary><b>⚙️ Edge Daemon &amp; Privacy-by-Design Specs</b></summary>
        <ul>
          <li><b>Zero-Unblurred Persistence:</b> Faces, windshields, and pedestrians are redacted irreversibly in RAM on the edge node prior to any disk write or S3 snapshot upload.</li>
          <li><b>Decoupled Tax Retention:</b> Settled parking sessions purge plate PII automatically while retaining immutable <code>§ 147 AO</code> accounting vouchers and zero-PII cryptographic purge audit logs.</li>
        </ul>
      </details>
      <br/>
      <a href="https://github.com/aymanmali/parkvektor-private-de"><img src="https://img.shields.io/badge/PUBLIC_REPO-181717?style=flat-square&logo=github&logoColor=white" alt="Public Repo"/></a>
      <img src="https://img.shields.io/badge/Independent_MVP-0EA5E9?style=flat-square" alt="Independent MVP"/>
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>
      <img src="https://img.shields.io/badge/ONNX_Runtime-005CED?style=flat-square&logo=onnx&logoColor=white" alt="ONNX"/>
      <img src="https://img.shields.io/badge/YOLO-111F68?style=flat-square&logo=yolo&logoColor=white" alt="YOLO"/>
      <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
      <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
    </td>
  </tr>
</table>

<p align="center">
  <sub><i>Note: ParkVektor Private DE is an independent R&amp;D project (fictional Musterdaten &amp; synthetic simulation only) and is not affiliated with or endorsed by any third-party hardware or payment vendors.</i></sub>
</p>

<br/>

<div align="center">
  <img src="./assets/section-opensource.svg" width="100%" alt="02 — Open-Source Ecosystem" />
</div>

<table>
  <tr>
    <td align="center" width="50%">
      <a href="https://github.com/aymanmali/quackboard"><img src="https://github.com/aymanmali.png" width="52" alt="QuackBoard"/></a>
      <h3><a href="https://github.com/aymanmali/quackboard">QuackBoard</a></h3>
      <img src="https://img.shields.io/badge/ROLE-CREATOR_//_MIT-10B981?style=flat-square&logo=github&logoColor=white&labelColor=0B1324" alt="Creator"/>
      <p>Open-source Tableau-like Business Intelligence platform powered by DuckDB-Wasm, Apache ECharts, and Next.js.</p>
    </td>
    <td align="center" width="50%">
      <a href="https://github.com/aymanmali/smart-parking-guidance-system"><img src="https://github.com/aymanmali.png" width="52" alt="Smart Parking Guidance System"/></a>
      <h3><a href="https://github.com/aymanmali/smart-parking-guidance-system">Smart Parking Guidance System</a></h3>
      <img src="https://img.shields.io/badge/ROLE-CREATOR_//_MIT-10B981?style=flat-square&logo=github&logoColor=white&labelColor=0B1324" alt="Creator"/>
      <p>Open-source 300-slot computer-vision parking guidance platform (YOLOv8, PyTorch, FastAPI, ESP32 C, KiCad PCB).</p>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <a href="https://github.com/CopilotKit/openfuse"><img src="https://github.com/CopilotKit.png" width="52" alt="OpenFuse"/></a>
      <h3><a href="https://github.com/CopilotKit/openfuse">OpenFuse</a></h3>
      <img src="https://img.shields.io/badge/ROLE-CONTRIBUTOR-38BDF8?style=flat-square&logo=github&logoColor=white&labelColor=0B1324" alt="Contributor"/>
      <p>CopilotKit's open-source personal agent with a browser, terminal, and files.</p>
    </td>
    <td align="center" width="50%">
      <a href="https://github.com/CopilotKit/OpenBot"><img src="https://github.com/CopilotKit.png" width="52" alt="OpenBot"/></a>
      <h3><a href="https://github.com/CopilotKit/OpenBot">OpenBot</a></h3>
      <img src="https://img.shields.io/badge/ROLE-CONTRIBUTOR-38BDF8?style=flat-square&logo=github&logoColor=white&labelColor=0B1324" alt="Contributor"/>
      <p>CopilotKit's open-source AI coworkers, each with a computer of its own.</p>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <a href="https://github.com/cline/cline"><img src="https://github.com/cline.png" width="52" alt="Cline"/></a>
      <h3><a href="https://github.com/cline/cline">Cline</a></h3>
      <img src="https://img.shields.io/badge/ROLE-CONTRIBUTOR-38BDF8?style=flat-square&logo=github&logoColor=white&labelColor=0B1324" alt="Contributor"/>
      <p>Autonomous coding agent as an IDE extension, CLI, and SDK.</p>
    </td>
    <td align="center" width="50%">
      <a href="https://github.com/PrefectHQ/fastmcp"><img src="https://github.com/PrefectHQ.png" width="52" alt="FastMCP"/></a>
      <h3><a href="https://github.com/PrefectHQ/fastmcp">FastMCP</a></h3>
      <img src="https://img.shields.io/badge/ROLE-CONTRIBUTOR-38BDF8?style=flat-square&logo=github&logoColor=white&labelColor=0B1324" alt="Contributor"/>
      <p>The fast, Pythonic way to build MCP servers and clients.</p>
    </td>
  </tr>
</table>

<br/>

<div align="center">
  <img src="./assets/section-telemetry.svg" width="100%" alt="03 — Stack Matrix & GitHub Telemetry" />
</div>

<div align="center">

<br/>

<p>
  <img src="https://skillicons.dev/icons?i=python,pytorch,sklearn,opencv,fastapi,ts,nextjs,postgres,docker,gcp,linux,githubactions,git,github&perline=14" alt="Core Engineering Toolchain" />
</p>

<p>
  <img src="https://img.shields.io/badge/LangGraph-0B1324?style=flat-square&logo=langchain&logoColor=38BDF8" alt="LangGraph"/>
  <img src="https://img.shields.io/badge/LangChain-0B1324?style=flat-square&logo=langchain&logoColor=10B981" alt="LangChain"/>
  <img src="https://img.shields.io/badge/Model_Context_Protocol_(MCP)-0B1324?style=flat-square&logo=modelcontextprotocol&logoColor=A855F7" alt="MCP"/>
  <img src="https://img.shields.io/badge/ONNX_Runtime-0B1324?style=flat-square&logo=onnx&logoColor=005CED" alt="ONNX Runtime"/>
  <img src="https://img.shields.io/badge/DuckDB--Wasm-0B1324?style=flat-square&logo=duckdb&logoColor=F59E0B" alt="DuckDB-Wasm"/>
  <img src="https://img.shields.io/badge/ESP32_ESP--IDF-0B1324?style=flat-square&logo=espressif&logoColor=E7352C" alt="ESP32"/>
  <img src="https://img.shields.io/badge/KiCad_PCB-0B1324?style=flat-square&logo=kicad&logoColor=314CB0" alt="KiCad"/>
</p>

<br/>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=aymanmali&theme=github_dark" width="96%" alt="GitHub Profile Summary" />

<br/><br/>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=aymanmali&theme=github_dark" width="47%" alt="Repositories per Language" />
&nbsp;
<img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=aymanmali&theme=github_dark&utcOffset=1" width="47%" alt="Productive Time" />

<br/><br/>

---

<code>SYS.EOF // © 2026 Ayman Ali • Applied AI @ DIT • Munich, Germany 🇩🇪</code>

</div>
