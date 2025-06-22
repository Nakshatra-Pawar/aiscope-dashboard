# AIscope Dashboard

> **AIscope** is an interactive Tableau Public workbook that transforms  
> **15 000 global AI-related job postings (2025 sample)** into one concise, filter-first view.  
> Instantly answer: **How big is the market?** • **Who pays what?** • **Which roles dominate?** • **How remote-friendly are employers?** • **Do large companies really offer better perks?**

<p align="center">
  <img src="images/dashboard.png" width="820" alt="AIscope dashboard preview">
</p>

---

## 📂 Repo Layout

aiscope-dashboard/
├── Dataset
├── aiscope_dashboard.twbx # Tableau workbook (Tableau Public 2024.1+)
├── dashboard-screenshot
├── README.md # you’re here

yaml
Copy
Edit
> `.DS_Store` files are ignored via `.gitignore` for a tidy repo.

---

## 🗃️ Dataset

| Source | Rows | Cols | License |
|--------|------|------|---------|
| **[Global AI Job Market & Salary Trends 2025 — Kaggle](https://www.kaggle.com/datasets/bismasajjad/global-ai-job-market-and-salary-trends-2025?utm_source=chatgpt.com)** | 15 000 | 11 | CC BY-SA |

Key columns used:

* `job_title`, `salary_usd`, `years_experience`, `experience_level`
* `remote_ratio` (0 = on-site, 50 = hybrid, 100 = fully remote)
* `company_size` (S < 50 • M 50–250 • L > 250)
* `benefits_score` (1-10 index)
* `posting_date`, `company_location`

---

## 🚀 Quick Start

```bash
# clone & enter the repo
git clone https://github.com/<your-user>/aiscope-dashboard.git
cd aiscope-dashboard