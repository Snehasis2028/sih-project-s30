# 🪪 SkillMatch - Portable Skill Passport & Fair Matchmaking Engine

An evidence-backed platform that converts verified academic coursework, open source projects, hackathon achievements, and accredited micro-credentials into a **verifiable, portable digital Skill Passport**. Matches students to **internships** and **multidisciplinary project teams** with **explainable evidence citations**, actionable skill gap roadmaps, and a **100% bias-shielded merit evaluation**.

---

## 🌟 Key Capabilities

1. **Multi-Source Evidence-Backed Skill Passport**:
   - Aggregates verified university coursework (syllabi, grades, course codes).
   - Verifies practical projects with GitHub commit tracking.
   - Captures objective competition / hackathon rankings (e.g. Smart India Hackathon awards).
   - Validates industry micro-credentials (AWS, Meta, Google) with cryptographic ledger hashes.
   - Portable export as verifiable **JSON-LD** and printable digital identity card with QR code.

2. **Explainable Internship Matching Engine**:
   - Calculates weighted match scores based on demonstrated competencies.
   - **Evidence Citations Drawer**: Explains precisely which specific course, repo, or certificate substantiates each required skill.
   - **Skill Gap Roadmaps**: Identifies missing competencies and recommends targeted learning pathways.

3. **Multidisciplinary Team Matchmaking**:
   - Evaluates functional domain complementarity to balance teams across UI/UX, AI/ML, Cloud Infrastructure, and Backend Engineering.
   - Computes a **Team Synergy Score** based on missing skills the student brings.

4. **100% Bias-Shielded Fairness Guarantee**:
   - Strips protected demographic attributes (gender, age, race, religion, socio-economic factors) and college prestige proxies (Tier-1 vs Tier-3) from evaluation algorithms.
   - Provides an interactive **Algorithmic Fairness Audit Log**.

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v16+)
- npm

### Installation & Execution
```bash
npm install
node server.js
```

Open your browser at:
```
http://localhost:5000
```
- **Home Portal**: `http://localhost:5000/index.html`
- **Skill Passport Studio**: `http://localhost:5000/profile.html`
- **Opportunities & Teams Hub**: `http://localhost:5000/opportunities.html`

---

## 📡 REST API Reference

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/api/health` | Service health and engine version |
| `GET` | `/api/sample-profiles` | Retrieve preset verified student personas |
| `GET` | `/api/passport/:id` | Retrieve candidate skill passport |
| `POST` | `/api/passport` | Create or update verified skill passport |
| `GET` | `/api/opportunities` | List all industry internship opportunities |
| `POST` | `/api/match/internships` | Compute explainable matches and evidence citations |
| `GET` | `/api/teams` | List multidisciplinary project/hackathon teams |
| `POST` | `/api/match/teams` | Compute team complementarity synergy scores |
| `POST` | `/api/teams` | Register a new multidisciplinary project team |
| `POST` | `/api/verify/credential` | Verify credential ID / hash authenticity on ledger |
| `GET` | `/api/fairness-audit` | Algorithmic transparency and neutrality report |