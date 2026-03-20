<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=30&pause=1000&color=00C2FF&center=true&vCenter=true&width=700&lines=ShieldGig;E-commerce+Protection;AI+Insurance" />

</div>

<p align="center">
<b>Understanding the Problem</b><br>
<i>Income instability in e-commerce delivery work</i>
</p>

---

# 📌 Problem Statement

E-commerce platforms like Amazon and Flipkart rely heavily on delivery partners for last-mile delivery.

But their income isn’t fixed.

They earn **per delivery**, which means:

👉 No deliveries = No income  

---

### ⚠️ The reality

Everyday conditions can suddenly stop their work:

- 🌧 Rain & floods  
- 🌡 Extreme heat  
- 🌫 Pollution  
- 🚧 Local restrictions  

When this happens, deliveries slow down or stop entirely.

---

```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'pie1': '#00C2FF', 'pie2': '#FF6B6B'}}}%%
pie title Weekly Income Reality
    "Active Earnings (~75%)" : 75
    "Income Loss (~25%)" : 25
```

---

# Why This Matters

India’s gig economy is growing fast — and e-commerce delivery is a big part of it.  

- Over **3.7 million delivery workers** rely on platforms like **Amazon, Flipkart, Swiggy, Zomato, Blinkit, Zepto**  
- Most depend on **daily earnings to survive**, meaning even **1–2 days of disruption** can hit their weekly income  
- External factors like **rain, floods, extreme heat, pollution, or local restrictions** can instantly stop deliveries  

Despite being essential, these workers have **no income protection**.  

ShieldGig aims to provide a **data-driven financial safety net** through **automated parametric insurance**.

---

# ⚡ Parametric Triggers

ShieldGig automatically monitors **measurable thresholds** and releases payouts when workers are affected by external disruptions.

- **Rainfall & Floods** 🌧 — triggers payouts if rainfall exceeds a set limit or flood alerts are issued in the delivery zone  
- **Extreme Heat** 🌡 — activates when temperatures rise above safe working thresholds for multiple hours  
- **Air Pollution** 🌫 — triggers compensation if AQI crosses unhealthy levels in affected regions  
- **Local Restrictions & Curfews** 🚧 — automatically compensates workers if government-imposed restrictions prevent deliveries  
- **Operational Downtime** ⚙️ — monitors delivery platform or route disruptions and triggers payouts for lost income  
- **AI Verification & Fraud Detection** 🤖 — confirms worker activity and validates eligibility, preventing false claims  
- **Automatic Wallet Credit** 💳 — payouts are instantly credited to the worker’s digital wallet  

---

# 🛡️ Proposed Concept: ShieldGig

ShieldGig is a **parametric micro-insurance platform** for e-commerce delivery gig workers.  
It provides **automatic payouts** when external disruptions affect earnings, without any manual claim process.

- Uses **environmental triggers** like heavy rain, floods, extreme heat, pollution, or local restrictions  
- **AI verifies worker activity** in the affected zone before releasing payouts  
- **Fraud detection** prevents misuse, ensuring fair and accurate compensation  
- **Automatic credit** of payouts reduces income instability for workers  

```mermaid
flowchart TD
    %% Sections
    subgraph User_Interaction
        FE[Frontend]
    end

    subgraph Core_Backend
        BE[Backend]
    end

    subgraph AI_Processing
        AI[AI Model]
        VAL[Validate]
    end

    subgraph Payment_Module
        PAY[Payment]
    end

    subgraph API_Section
        API[API]
        TR[Trigger]
    end

    %% Connections
    FE <--> BE
    BE --> AI
    AI --> VAL
    VAL --> PAY
    API --> TR
    TR --> BE
    AI --> BE

    %% Labeled arrows (optional readability)
    FE -->|User Requests| BE
    BE -->|Data for AI| AI
    AI -->|Validation Input| VAL
    VAL -->|Process Payment| PAY
    API -->|External Call| TR
    TR -->|Trigger Backend| BE
    AI -->|Feedback| BE
```

---

# Workflow Scenario: E-commerce Delivery Gig Workers

## Example Case

Worker: Priya, a delivery partner in Mumbai  
Weekly Earnings: ₹7,000  

Incident: Heavy rainfall floods her delivery zone for 3 days, causing ₹2,500 income loss  

**Weather API Detection:**  
Real-time monitoring detects extreme rainfall above the defined threshold.

**Parametric Trigger:**  
The system validates that Priya’s delivery zone meets the payout conditions.

**AI Validation:**  
AI verifies her activity data to confirm she was assigned deliveries and affected by the disruption.

**Fraud Prevention:**  
System checks for anomalies to prevent misuse.

**Automatic Payout Initiation:**  
The platform calculates compensation based on expected income loss.

**Instant Compensation:**  
Priya receives ₹1,800 in her digital wallet automatically.

No manual claim required – payouts are fully automated.

---

# Visual System Workflow

<p align="center">
<img src="images/visualworkflow.jpg" width="850">
</p>

---

# System Architecture

<p align="center">
<img src="images/systemarchiture.jpg" width="850">
</p>

## Architecture Components:
**Client Interface:**
Delivery partner dashboard
Policy enrollment
Coverage status tracking
Live activity monitoring

**Backend Node:**
Policy management
Worker activity tracking
API polling
Event monitoring
Assignment timestamp tracking
Payout processing control

**Defense Layer:**
GPS validation
Route distance check
Speed vs distance verification
VPN / proxy detection
Device ID verification
Duplicate request detection
Assignment time verification
Event time verification
Fraud prevention checks

**Risk Engine:**
Calculates geographic risk score
Predicts disruption probability
Uses historical weather data
Identifies flood-prone zones
Determines dynamic premium pricing
Determines payout amount

### Data Oracles:
**External data sources:**
Weather API
Flood alert API
Government restriction alerts
AQI / pollution APIs
Maps / location API
Platform delivery data API

**AI Agent:**
Fraud detection
Risk prediction
Payout validation
Anomaly detection
Eligibility verification

**Trigger Engine:**
Evaluates incoming environmental data
Checks parametric rules
Matches event with worker location
Validates assignment before event
Activates payout trigger

**Event Validation Module:**
Checks event time
Checks worker location
Checks delivery assignment
Checks zone eligibility
Confirms disruption impact

**Payment Gateway:**
Wallet credit
Insurance payout
Blocked payout (fraud)
Delayed payout (review)
Secure transaction processing

**Feedback Loop:**
Backend ↔ AI Agent
AI ↔ Defense Layer
AI ↔ Risk Engine

**Used for:**
Improving fraud detection
Improving risk scoring
Preventing liquidity attack
Increasing payout accuracy

---

# AI & Logic Integration Strategy

**Risk Prediction Engine:**

Historical weather data  
Flood-prone delivery zones  
Seasonal delivery disruptions  

**Dynamic Pricing Logic:**

Geographic risk level  
Weather severity  
Number of assigned deliveries  
Expected daily earnings  

**Fraud Detection:**

GPS validation  
Route distance check  
Event API cross-check  
Duplicate request detection  
Assignment time verification

---

# Development Roadmap

**Phase 1:**

Concept design
System architecture planning
Workflow design
Parametric insurance modeling
Risk engine design
Fraud detection strategy
GPS validation logic
Defense layer design

**Phase 2:**

Backend development
API integration
Weather / Flood / Restriction APIs
Event trigger engine
Risk engine implementation
AI agent integration
GPS tracking module
Fraud detection module
Assignment tracking system
Event validation module

**Phase 3:**

Automation flow
Parametric trigger automation
Auto validation
Auto payout system
Payment gateway integration
Fraud prevention checks
AI feedback loop
Testing & simulation
Cloud deployment
Monitoring & logging
Production release

---

# Team

| Member | Role |
|------|------|
| *Vamsi Krishna Reddy* | System Architecture & Frontend |
| *Ashraf* | Research & Policy Designer|
| *Kamesh Prasad* | Backend & Application Development|
| *Vishnu Vamsi* | Data Collection |
| *Hari Venkata* | AI / ML |

---