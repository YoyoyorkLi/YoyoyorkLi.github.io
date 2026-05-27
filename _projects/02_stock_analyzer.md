---
name: Stock Sentiment Analyzer
tools: [Natural Language Processing]
description: A dashboard that pulls and analyzes live financial headlines.
image: assets/pngs/stock.png
---

### Overview

---
This dashboard pulls and analyzes financial headlines of any stock in the past 7 trading days. 

<br>
### Try the App!

*(If the Space is sleeping, click "Restart Space" to wake it up!)*

<iframe
    id="gradio-app"
    src="https://yoyoyork-stock-headline-analyzer.hf.space"
    frameborder="0"
    width="100%"
    height="500"
></iframe>

<script>
  // 1. Grab the iframe using the assigned ID
  const iframe = document.getElementById('gradio-app');
  // 2. Point to the correct stock analyzer URL
  const baseUrl = "https://yoyoyork-stock-headline-analyzer.hf.space";
  
  function syncTheme() {
    // Checks if your main portfolio site is in dark mode
    const isDark = document.documentElement.getAttribute('data-theme') === 'dark';
    const targetUrl = isDark ? baseUrl + "/?__theme=dark" : baseUrl + "/?__theme=light";
    
    // Only reload the iframe if the theme actually changed
    if (iframe.src !== targetUrl) {
      iframe.src = targetUrl;
    }
  }

  // Run immediately on page load
  syncTheme();

  // Watch the portfolio site's HTML tag for theme toggles
  const observer = new MutationObserver((mutations) => {
    mutations.forEach((mutation) => {
      if (mutation.attributeName === 'data-theme') {
        syncTheme();
      }
    });
  });

  observer.observe(document.documentElement, { attributes: true });
</script>
---