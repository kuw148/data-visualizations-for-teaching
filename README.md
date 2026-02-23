# Data Visualizations for Teaching

This repository contains interactive, browser-native data visualizations developed for university-level instruction in communication research methods, media studies, rhetoric, digital literacy, and network analysis.

All materials are designed to be:

- **Open source**
- **Institution-independent**
- **Browser-native (HTML / CSS / JavaScript)**
- **Embeddable via iframe in any LMS**
- **Explicit in their geometric and scaling assumptions**

The goal is not simply to display data, but to make the *structure of representation* visible to students.

---

## Why This Repository Exists

University teaching often relies on proprietary visualization platforms (e.g., Tableau, Power BI, institutional dashboards). These systems are typically:

- License-bound  
- Platform-dependent  
- Non-portable across institutions  
- Opaque in their layout and scaling logic  

This repository takes a different approach.

All visualizations are built using:

- **D3.js** (primary visualization framework)
- Plain HTML and CSS
- Self-contained JSON or CSV datasets

Each module can be hosted statically (e.g., GitHub Pages) and embedded anywhere without institutional dependency.

---

## Pedagogical Principles

### 1. Geometric Integrity

Aspect ratios, scales, and coordinate systems are explicitly defined.  
Padding and layout models are controlled deliberately.

When teaching about misleading data visualizations, the visualizations themselves must not be distorted by container quirks or hidden layout behavior.

### 2. Transparency of Representation

Students should be able to see:

- How data maps onto visual variables  
- Where scaling decisions are made  
- How thresholds alter interpretation  
- How representational choices frame meaning  

In many cases, the code itself is part of the lesson.

### 3. Interactive Exploration

Where appropriate, modules include:

- Adjustable thresholds and parameters  
- Node and edge toggles  
- Hover annotations  
- Structured explanatory notes  

The aim is to allow students to explore how analytical conclusions shift when representational assumptions change.

---

## Current Modules

### Simulated Subreddit Network Analysis (D3)

An instructional dataset including:

- 10 simulated subreddits  
- Subscriber counts  
- Daily post volume  
- Human-to-bot account ratios  
- Indexed subscriber overlap (0–1 scale)  
- Cross-post volume between subreddit pairs  

The interactive network visualization demonstrates:

- Node size mapped to subscriber count or daily post volume  
- Node color mapped to human-to-bot ratio  
- Edge thickness mapped to overlap or cross-post volume  
- Adjustable edge threshold to reduce visual noise  
- Force-directed layout with drag and zoom  

This module is intended for communication research methods courses introducing:

- Network analysis  
- Data visualization design  
- Representational bias  
- Interpretive framing in digital data  

---

## How to Use

1. Host the HTML module using GitHub Pages (or another static host).
2. Embed in your LMS using an iframe:

```html
<iframe 
  src="https://yourusername.github.io/Data-visualizations-for-teaching/path/to/module.html"
  width="100%" 
  height="720" 
  style="border:none;">
</iframe>
