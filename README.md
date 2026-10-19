# PSI Median Runner

A single-page tool that runs Google PageSpeed Insights several times for mobile and desktop, then reports the **median** of each metric and how much the runs varied. A single PSI test can be off by 10 points or more, so the median is the number worth reporting.

## Features

- 3 or 5 runs per device, with mobile and desktop running side by side. You can cancel a test while it runs.
- Median score plus the median and range of FCP, LCP, TBT, CLS and Speed Index.
- A stability rating (Stable / Some variance / Unstable) and the metric that moved most.
- Real-user (Chrome UX Report) data when the site has it.
- "Where the weight comes from": requests, transfer size, unused code and JS CPU time, grouped by plugin, theme or third-party service.
- Fixes ranked by impact. Only issues that failed in at least half the runs are listed.
- The most representative run, which you can open in Lighthouse Viewer or download.
- A downloadable results report. It never includes your API key.
- Detection of runs that Google served from its cache.

## Usage

1. Get a free PageSpeed Insights API key: Google Cloud Console → Credentials → Create credentials → API key. Restrict it to the PageSpeed Insights API.
2. Open `index.html` in a browser, or use the GitHub Pages link if it's enabled.
3. Paste a URL and your key, then click **Run tests**.

The key is stored only in your own browser (localStorage) and is sent only to Google's API.

---

© Created by Timak
