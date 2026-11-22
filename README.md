# Mini Google 1998 🔍

A lightweight, single-file search engine simulation comparing the **"Old Way (1997)"** of ranking web pages using keyword frequency against the **"Surfer Way (1998)"** using a Monte Carlo PageRank random surfer simulation.

Built for a first-year AI lab — zero dependencies, zero installation, runs completely offline in any web browser.

---

## 🌟 Overview

Before PageRank was introduced by Larry Page and Sergey Brin in 1998, search engines ranked pages primarily by **keyword frequency (TF)**. This led to widespread "keyword stuffing" where spam websites repeated words dozens of times to take the top rank.

**Mini Google 1998** illustrates why link-based authority changed the web:
- **Old Way (1997):** Counts how many times the search word appears in the page text as a whole word (case-insensitive). Highest count ranks first.
- **Surfer Way (1998):** Simulates a random surfer taking **100,000 steps** on the web graph:
  - **15%** chance: The surfer gets bored and teleports to any random page.
  - **85%** chance: The surfer clicks one of the current page's outgoing links at random (or teleports if at a dead end).
  - Scores are calculated as:
    $$\text{Surfer Score} = \left(\frac{\text{Visits}}{100{,}000}\right) \times 100\%$$
  - Also displays **"Links in: N"** (the number of other pages that link to that page).

---

## 🚀 How to Run

1. Clone or download this repository.
2. Double-click `index.html` to open it in Chrome, Safari, Firefox, or Edge.
3. No build tools, Node.js, Python, or local web server required!

---

## 🎯 Example Queries Included

- **🍕 pizza:** Demonstrates how keyword-stuffed spam (`super-cheap-pizza-deals.com`) dominates 1997 rankings, while authentic NY pizza authority (`joespizzanyc.com`) wins 1998 PageRank.
- **🏏 cricket:** Shows international cricket news portal (`cricinfo-world.org`) outranking spam pages.
- **🎬 movie:** Compares film databases (`cinema-database.org`) against movie download spam.
- **📝 exam:** Shows academic university portals (`university-academics.edu`) outranking cheat-sheet spam sites.

---

## 🛠️ Tech Stack

- **HTML5** (Semantics & responsive two-column layout)
- **CSS3** (1998 retro Google styling with modern clean UX)
- **Vanilla JavaScript** (Linear, well-commented, beginner-friendly simulation)
