<div align="center">

<img src="./assets/hero-aurora.svg" width="100%" alt="Ayman Ali — AI Engineer" />

<br/>

<p align="center">
  <a href="mailto:ayman.m.ali148@gmail.com">
    <img src="https://img.shields.io/badge/Email-ayman.m.ali148%40gmail.com-18181B?style=flat-square&logo=gmail&logoColor=white&labelColor=09090B" alt="Email" />
  </a>
  &nbsp;
  <a href="https://github.com/aymanmali">
    <img src="https://img.shields.io/badge/GitHub-@aymanmali-18181B?style=flat-square&logo=github&logoColor=white&labelColor=09090B" alt="GitHub" />
  </a>
  &nbsp;
  <img src="https://img.shields.io/badge/Location-Munich,_Germany-18181B?style=flat-square&labelColor=09090B" alt="Munich, Germany" />
</p>

</div>

---

## About

I'm **Ayman**, an **AI Engineer** and **M.Eng. student in Applied AI for Digital Production Management** at **DIT (Germany)**, with a **B.Sc. in Mechatronics Engineering** and experience in **Project Management**.

I design and ship **Agentic AI systems** (`LangGraph`, `LangChain`, `MCP`), **Computer Vision & Deep Learning pipelines** (`PyTorch`, `YOLOv8`, `ONNX`, `Scikit-learn`), and cloud-deployed **FastAPI & Docker** services that bridge software intelligence with real-world engineering systems.

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>Agentic AI &amp; LLM Engineering</h4>
      <p>Stateful multi-step agent graphs, Model Context Protocol (MCP) servers and transports, dynamic tool calling, and automated evaluation workflows.</p>
      <p><code>LangGraph</code> · <code>LangChain</code> · <code>FastMCP</code> · <code>Tool Calling</code> · <code>Evals</code></p>
    </td>
    <td width="50%" valign="top">
      <h4>Computer Vision &amp; Machine Learning</h4>
      <p>Multi-camera object detection, calibrated ROI classification, multi-frame OCR, temporal hysteresis, and in-RAM privacy redaction at the edge.</p>
      <p><code>PyTorch</code> · <code>YOLOv8</code> · <code>ONNX Runtime</code> · <code>OpenCV</code> · <code>Scikit-learn</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4>Backend, Data &amp; Cloud</h4>
      <p>High-concurrency REST and WebSocket APIs, in-browser analytical SQL engines, relational storage, and containerized cloud deployments.</p>
      <p><code>FastAPI</code> · <code>DuckDB-Wasm</code> · <code>PostgreSQL</code> · <code>Docker</code> · <code>GCP</code></p>
    </td>
    <td width="50%" valign="top">
      <h4>Engineering Foundation</h4>
      <p>M.Eng. Applied AI @ DIT (Germany) and B.Sc. Mechatronics Engineering — combining embedded hardware, firmware, and industrial systems thinking.</p>
      <p><code>Python</code> · <code>TypeScript</code> · <code>ESP32 C</code> · <code>RS-485</code> · <code>KiCad PCB</code></p>
    </td>
  </tr>
</table>

---

## Featured Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/aymanmali/smart-parking-guidance-system">Smart Parking Guidance System</a></h3>
      <p><sub><b>300-Slot Computer Vision &amp; Embedded Guidance Platform · Inspired by 2019 Galleria40 Mall (LEED) Deployment</b></sub></p>
      <p>End-to-end automated parking guidance platform across 4 zones, 12 edge cameras, 2 entrance counter displays, and 4 internal intersection directional screens.</p>
      <ul>
        <li><b>Edge Vision:</b> YOLOv8 detection in PyTorch paired with calibrated OpenCV ROI polygons, a PyTorch CNN classifier, and temporal hysteresis.</li>
        <li><b>Real-Time Routing:</b> FastAPI REST + WebSocket server driving live zone/intersection guidance via an MQTT and RS-485 (<code>CRC-16</code>) hardware bridge.</li>
        <li><b>Hardware &amp; Signage:</b> React operator dashboard and LED signage simulator, ESP32 Embedded C (<code>ESP-IDF</code>) firmware, and a custom KiCad PCB (<code>SPG-CTRL-v1</code>).</li>
      </ul>
      <p><code>Python</code> · <code>PyTorch</code> · <code>YOLOv8</code> · <code>OpenCV</code> · <code>FastAPI</code> · <code>ESP32 C</code> · <code>KiCad</code></p>
      <p>
        <a href="https://smart-parking-guidance-system.vercel.app"><img src="https://img.shields.io/badge/Live_Demo_↗-10B981?style=flat-square&logo=vercel&logoColor=white" alt="Live Demo"/></a>
        &nbsp;
        <a href="https://github.com/aymanmali/smart-parking-guidance-system"><img src="https://img.shields.io/badge/Repository_↗-18181B?style=flat-square&logo=github&logoColor=white" alt="Repository"/></a>
      </p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/aymanmali/quackboard">QuackBoard</a></h3>
      <p><sub><b>Open-Source Tableau-Style BI &amp; In-Browser OLAP Platform · DuckDB-Wasm &amp; Next.js 15</b></sub></p>
      <p>Zero-setup Business Intelligence web application for instant local file analytics in the browser and live read-only SQL dashboards.</p>
      <ul>
        <li><b>Hybrid Query Engine:</b> In-browser DuckDB-Wasm Web Worker over CSV, Parquet, Excel, and JSON files plus AES-256-GCM encrypted PostgreSQL &amp; MySQL connections.</li>
        <li><b>Visual Chart Studio:</b> Drag-and-drop Dimension &amp; Measure shelves compiling to dialect-aware SQL across 9 Apache ECharts visualization types and an ad-hoc SQL Lab.</li>
        <li><b>Interactive Dashboards:</b> Drag-and-resize grid layouts, global filters, click-to-cross-filter across charts, portable <code>.quackboard.json</code> export, and IndexedDB persistence.</li>
      </ul>
      <p><code>TypeScript</code> · <code>DuckDB-Wasm</code> · <code>Next.js 15</code> · <code>Apache ECharts</code> · <code>PostgreSQL</code></p>
      <p>
        <a href="https://quackboard-rosy.vercel.app"><img src="https://img.shields.io/badge/Live_Demo_↗-10B981?style=flat-square&logo=vercel&logoColor=white" alt="Live Demo"/></a>
        &nbsp;
        <a href="https://github.com/aymanmali/quackboard"><img src="https://img.shields.io/badge/Repository_↗-18181B?style=flat-square&logo=github&logoColor=white" alt="Repository"/></a>
      </p>
    </td>
  </tr>
  <tr>
    <td colspan="2" valign="top">
      <h3><a href="https://github.com/aymanmali/parkvektor-private-de">ParkVektor Private DE</a></h3>
      <p><sub><b>Barrierless ANPR Private Parking &amp; Ticketing MVP for Germany · DSGVO Privacy-by-Design</b></sub></p>
      <p>An independent barrier-free ANPR private parking and ticketing platform designed around German civil/tax workflows (<code>BGB</code>, <code>§ 147 AO</code>, <code>§ 39 StVG</code>) and edge privacy redaction.</p>
      <ul>
        <li><b>Hybrid Edge AI &amp; Smart ANPR:</b> Standalone Python Edge AI daemon (RTSP/ONVIF ingest, ONNX Runtime YOLO vehicle/plate detection, EU/DE slot+CTC plate OCR with IoU multi-frame voting, German <code>FE-Schrift</code> normalization, in-RAM face/windshield blurring, SQLite WAL offline sync) plus webhook adapters for commercial ANPR cameras.</li>
        <li><b>Tariffs, Payments &amp; DSGVO Auto-Purge:</b> Flexible weekday/weekend tariffs, pluggable Stripe checkout (SEPA, Apple Pay, Google Pay, PayPal) with <code>19% MwSt.</code> PDF invoices, and automated raw-plate/snapshot purging with zero-PII audit logs.</li>
        <li><b>Bilingual Portals (DE/EN):</b> Next.js Driver QR Pay &amp; AutoPay wallets, German QWERTZ Pay-on-Foot Kiosk, Tenant Validation, Driver <i>Widerspruchsportal</i>, and Operator Admin / <code>§ 39 StVG</code> QA dashboard.</li>
      </ul>
      <p><code>Python</code> · <code>FastAPI</code> · <code>ONNX Runtime</code> · <code>YOLO</code> · <code>Next.js</code> · <code>PostgreSQL</code> · <code>Stripe</code> · <code>Docker</code></p>
      <p>
        <a href="https://parkvektor-private-de.vercel.app"><img src="https://img.shields.io/badge/Live_Demo_↗-10B981?style=flat-square&logo=vercel&logoColor=white" alt="Live Demo"/></a>
        &nbsp;
        <a href="https://github.com/aymanmali/parkvektor-private-de"><img src="https://img.shields.io/badge/Repository_↗-18181B?style=flat-square&logo=github&logoColor=white" alt="Repository"/></a>
        &nbsp;
        <img src="https://img.shields.io/badge/Independent_MVP-27272A?style=flat-square" alt="Independent MVP"/>
      </p>
    </td>
  </tr>
</table>

<p align="center">
  <sub><i>ParkVektor Private DE is an independent R&amp;D project (fictional Musterdaten &amp; synthetic simulation only) and is not affiliated with or endorsed by any third-party hardware or payment vendors.</i></sub>
</p>

---

## Open Source

<table>
  <tr>
    <td align="center" width="50%">
      <br/>
      <a href="https://github.com/aymanmali/quackboard"><img src="https://github.com/aymanmali.png" width="48" alt="QuackBoard"/></a>
      <h4><a href="https://github.com/aymanmali/quackboard">QuackBoard</a></h4>
      <img src="https://img.shields.io/badge/Creator-10B981?style=flat-square" alt="Creator"/>
      <p><sub>Open-source Tableau-like BI platform powered by DuckDB-Wasm, Apache ECharts, and Next.js.</sub></p>
    </td>
    <td align="center" width="50%">
      <br/>
      <a href="https://github.com/aymanmali/smart-parking-guidance-system"><img src="https://github.com/aymanmali.png" width="48" alt="Smart Parking Guidance System"/></a>
      <h4><a href="https://github.com/aymanmali/smart-parking-guidance-system">Smart Parking Guidance System</a></h4>
      <img src="https://img.shields.io/badge/Creator-10B981?style=flat-square" alt="Creator"/>
      <p><sub>Open-source 300-slot computer-vision parking guidance platform (YOLOv8, PyTorch, FastAPI, ESP32 C, KiCad).</sub></p>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <br/>
      <a href="https://github.com/CopilotKit/openfuse"><img src="https://github.com/CopilotKit.png" width="48" alt="OpenFuse"/></a>
      <h4><a href="https://github.com/CopilotKit/openfuse">OpenFuse</a></h4>
      <img src="https://img.shields.io/badge/Contributor-27272A?style=flat-square" alt="Contributor"/>
      <p><sub>CopilotKit's open-source personal agent with a browser, terminal, and files.</sub></p>
    </td>
    <td align="center" width="50%">
      <br/>
      <a href="https://github.com/CopilotKit/OpenBot"><img src="https://github.com/CopilotKit.png" width="48" alt="OpenBot"/></a>
      <h4><a href="https://github.com/CopilotKit/OpenBot">OpenBot</a></h4>
      <img src="https://img.shields.io/badge/Contributor-27272A?style=flat-square" alt="Contributor"/>
      <p><sub>CopilotKit's open-source AI coworkers, each with a computer of its own.</sub></p>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <br/>
      <a href="https://github.com/cline/cline"><img src="https://github.com/cline.png" width="48" alt="Cline"/></a>
      <h4><a href="https://github.com/cline/cline">Cline</a></h4>
      <img src="https://img.shields.io/badge/Contributor-27272A?style=flat-square" alt="Contributor"/>
      <p><sub>Autonomous coding agent as an IDE extension, CLI, and SDK.</sub></p>
    </td>
    <td align="center" width="50%">
      <br/>
      <a href="https://github.com/PrefectHQ/fastmcp"><img src="https://github.com/PrefectHQ.png" width="48" alt="FastMCP"/></a>
      <h4><a href="https://github.com/PrefectHQ/fastmcp">FastMCP</a></h4>
      <img src="https://img.shields.io/badge/Contributor-27272A?style=flat-square" alt="Contributor"/>
      <p><sub>The fast, Pythonic way to build MCP servers and clients.</sub></p>
    </td>
  </tr>
</table>

---

## Technical Stack

| Programming &amp; APIs | AI &amp; Computer Vision | Agentic AI &amp; LLMs | Cloud &amp; Embedded |
| :--- | :--- | :--- | :--- |
| Python · TypeScript | PyTorch · Scikit-learn | LangGraph · LangChain | Docker · GCP · Linux |
| FastAPI · REST · WebSockets | YOLOv8 · ONNX Runtime | Model Context Protocol (MCP) | GitHub Actions CI/CD |
| SQL · PostgreSQL · DuckDB-Wasm | OpenCV · ROI &amp; OCR Pipelines | Tool Calling · Evals | ESP32 C (`ESP-IDF`) · KiCad |

<br/>

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=aymanmali&theme=github_dark" width="96%" alt="GitHub Profile Summary" />

<br/><br/>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=aymanmali&theme=github_dark" width="47%" alt="Repositories per Language" />
&nbsp;
<img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=aymanmali&theme=github_dark&utcOffset=1" width="47%" alt="Productive Time" />

<br/><br/>

<sub>© 2026 Ayman Ali · Munich, Germany</sub>

</div>
