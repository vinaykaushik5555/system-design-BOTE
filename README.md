# 📊 Back-of-the-Envelope (BOTE) System Design Template

A comprehensive **Excel-based calculator** to quickly estimate traffic, storage, compute, bandwidth, and scaling needs during **system design interviews** or real-world architecture planning.

---

## 🚀 Features
- **Traffic Calculations** — DAU → Events/day → QPS_avg → QPS_peak → concurrency.
- **Storage Estimation** — Daily, yearly, with replication.
- **Bandwidth** — Peak egress in Bps, MBps, monthly TB.
- **Compute** — CPU cores needed with headroom.
- **Database Sharding** — Reads/writes per node → required shards/nodes.
- **Cache Sizing** — Based on TTL and item size.
- **Cost Projection** — Storage, compute, and egress monthly costs.
- **Growth Projection** — Multi-year DAU growth charts for QPS and storage.
- **Latency Budgeting** — Allocate SLA across components.
- **Scenario Analysis** — Compare base, 2×, and 5× load instantly.
- **Checklist** — Covers functional and non-functional requirements.
- **CheatSheet & Glossary** — Powers of 10, Indian numbering (Lakhs/Crores), byte units, and term definitions.

---

## 📂 Tabs Overview & Usage

### 1️⃣ **BOTE_System_Design**
Main input/output sheet.
- **Column B** — Enter your assumptions (DAU, actions/user/day, payload size, peak multiplier, etc.).
- Outputs in **Column E** auto-calculate:
  - Events/day
  - QPS (avg & peak)
  - Concurrency
  - Storage (daily/yearly/replicated)
  - Bandwidth & compute cores
  - DB shards/nodes
  - Cache capacity

**Tip:** Keep numbers rounded for quick mental validation.

---

### 2️⃣ **CheatSheet**
- Powers of 10 for users & storage.
- Indian units: Lakh, Crore alongside Billions/Trillions.
- Memory units in base-10 (KB, MB, GB, TB, PB).

---

### 3️⃣ **Glossary**
- Definitions and full forms of common system design terms.
- Example:  
  `QPS = Queries Per Second`  
  `RF = Replication Factor`

---

### 4️⃣ **Cost**
- Editable unit prices for storage, compute, and egress.
- Linked to main sheet outputs for automatic cost estimation.
- Update prices for AWS/GCP/Azure before use.

---

### 5️⃣ **Growth**
- Project DAU growth across multiple years.
- See impact on QPS_peak and yearly replicated storage.
- Includes charts for trends.

---

### 6️⃣ **LatencyBudget**
- Define total SLA (e.g., 300 ms).
- Allocate budget % to each tier (client, API, DB, cache, etc.).
- Auto-calculates ms per tier.
- Check sum of % = 100%.

---

### 7️⃣ **Checklist**
- Functional & non-functional design points.
- Yes/No dropdown for each.
- Helps avoid missing critical design aspects.

---

### 8️⃣ **Scenarios**
- Compare base, 2×, and 5× load.
- Instant calculation of QPS_peak, cores, and DB nodes.
- Visual chart for comparison.

---

## 🛠 How to Use in an Interview
1. **Open `BOTE_System_Design_Template_v4.xlsx`.**
2. Start in **BOTE_System_Design** tab → enter assumptions.
3. Move to **LatencyBudget** → distribute SLA.
4. Check **Cost** for budget feasibility.
5. Use **Growth** to show scale-up impact.
6. Test **Scenarios** for load surges.
7. Review **Checklist** before final design presentation.

---

## 📥 Download & Open
You can open it with:
- Microsoft Excel (preferred)
- Google Sheets (upload as `.xlsx` for formulas to work)
- LibreOffice (some chart formatting may differ)

---

## 📸 Example
> (Add screenshots from the Excel file showing key tabs.)

---

## 📄 License
MIT License – Free for personal and commercial use.

---

## 🤝 Contributing
Pull requests for improvements (e.g., more formulas, cloud provider-specific cost sheets) are welcome!
