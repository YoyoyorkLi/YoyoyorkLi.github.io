---
name: Stock Sentiment Analyzer
tools: [Natural Language Processing]
description: A dashboard that pulls and analyzes live financial headlines.
image: assets/pngs/stock.png
---
### Overview
---
This dashboard pulls and analyzes financial headlines of any stock in the past 7 trading days, weighting each headline by recency and sentiment. 
<br>
### Try the App!
*(If the Space is sleeping, click the link below to wake it up, then reload this page.)*

<a href="https://yoyoyork-stock-headline-analyzer.hf.space" target="_blank"> Open / Wake the Space</a>

<iframe
id="gradio-app"
src="https://yoyoyork-stock-headline-analyzer.hf.space"
frameborder="0"
width="100%"
height="500"
></iframe>
<script>
const iframe = document.getElementById('gradio-app');
const baseUrl = "https://yoyoyork-stock-headline-analyzer.hf.space";
function syncTheme() {
  const isDark = document.documentElement.getAttribute('data-theme') === 'dark';
  const targetUrl = isDark ? baseUrl + "/?__theme=dark" : baseUrl + "/?__theme=light";
  if (iframe.src !== targetUrl) {
    iframe.src = targetUrl;
  }
}
syncTheme();
const observer = new MutationObserver((mutations) => {
  mutations.forEach((mutation) => {
    if (mutation.attributeName === 'data-theme') {
      syncTheme();
    }
  });
});
observer.observe(document.documentElement, { attributes: true });
</script>
<br>