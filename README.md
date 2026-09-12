# Talent Intelligence Engine- 
Built for TA teams who want market intelligence without the $5K/year price tag.

Scan competitor companies for market signals (layoffs, RTO changes, leadership changes) using Gemini API + Google Apps Script.

**[Live Demo](https://bilal127.github.io/talent-intelligence-engine/) | [GitHub](https://github.com/bilal127/talent-intelligence-engine)**

---

## What It Does

Enter company names → Click "Scan" → Get:
- Market signals (layoffs, RTO, leadership changes)
- Talent mapping (which divisions affected, tech stacks, outreach hooks)
- Real-time results in Google Sheets

---

## How It Works

1. Add company names to Google Sheet
2. Click menu: 🔍 Intelligence → Run Market Scan
3. Gemini API searches the web
4. Results auto-populate in two sheets
5. Done in ~60 seconds

---

## What Costs Money (Gemini API)**

⚠️ Gemini API — Paid after free trial

Here's the exact breakdown:

First month: You get $5 free credits just for signing up
That $5 covers: Roughly 100-200 scans (depending on company count)
After $5 runs out: You pay actual usage
Input tokens: ~$0.075 per 1M tokens
Output tokens: ~$0.30 per 1M tokens

Real cost for your use case:

Scanning 5 companies 1x/week = ~$20-30/month
Scanning 5 companies daily = ~$100-150/month
Scanning 15 companies 1x/week = ~$40-60/month

vs. Competitors:

LinkedIn Talent Insights = $5,000+/year
Talent Neuron = $10,000+/year
This system = $240-600/year

---

## Setup (15 minutes)

1. Create Google Sheet named "Talent Intelligence Engine"
2. Add header row: Company | Tech Stack | Target Region | Priority Signals | Last Scanned | Status
3. Add 3-5 companies
4. Get Gemini API key: https://aistudio.google.com
5. Go to Extensions → Apps Script
6. Paste code from `apps_script_code.gs`
7. Replace `YOUR_API_KEY_HERE` with your actual key
8. Save and refresh sheet
9. Click 🔍 Intelligence → Run Market Scan

---

## Results

**Input:** Scan for Flipkart, Swiggy, Freshworks

**Output:**
- Market Radar: 8 signals found (layoffs, RTO, leadership changes)
- Talent Map: 6 talent opportunities with outreach hooks
- All with confidence scores and timestamps

---

## Cost

**Setup:** Free  
**Monthly:** $0-50 (after $5 free credit, then ~$0.30 per million API tokens)  
**vs Competitors:** LinkedIn Talent Insights costs $5,000+/year

---

## Tech Stack

- Google Sheets (storage)
- Google Apps Script (automation)
- Gemini API (AI + web search)
- GitHub Pages (web demo)

---

## FAQ

**Q: Can anyone use this?**  
A: Yes. Just need Gmail account and Gemini API key (free).

**Q: How accurate?**  
A: 70-90% (AI-based, always verify with primary sources).

**Q: Can I customize it?**  
A: Yes. Edit the `buildQueries()` function in Apps Script to add/change search queries.

**Q: Can my team use it?**  
A: Yes. Share the Google Sheet. One API key powers all searches.

---
