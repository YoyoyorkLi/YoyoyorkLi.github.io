---
name: AI-Powered Classroom Translator
tools: [Audio Processing, Open Sourced Model]
description: A free audio transcription and translation web app built for immigrant students in Tijuana.
image: assets/pngs/whisper.png
---
### Overview
---
In collaboration with the [LAS Global Leaders Program](https://las.illinois.edu/resources/international/globallearning/leaders), I worked with Tijuana's education department to support immigrant middle school students. 
To help bridge language barriers between students and faculty, I developed a free AI-powered translation web app that transcribes and translates live or recorded audio between English, Spanish, and Haitian Creole.
<br>
### Try the App!
*(If the Space is sleeping, click the link below to wake it up, then reload this page.)*

<a href="https://yoyoyork-on-demand-spanish-translator.hf.space" target="_blank"> Open / Wake the Space</a>

<div style="width: 100%; border-radius: 10px; overflow: hidden; border: 1px solid #888; margin-bottom: 30px;">
<iframe
id="gradio-app"
src=""
frameborder="0"
width="100%"
height="750"
style="border:none;"
></iframe>
</div>
<script>
const iframe = document.getElementById('gradio-app');
const baseUrl = "https://yoyoyork-on-demand-spanish-translator.hf.space";
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