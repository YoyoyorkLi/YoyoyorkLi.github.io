---
name: AI-Powered Classroom Translator
tools: [Audio Processing, Open Sourced Model]
description: A free audio transcription and translation web app built for immigrant students in Tijuana.
image: assets/pngs/whisper.png # Placeholder: Replace with a screenshot of your app!
---

### Overview

---
In collaboration with the [LAS Global Leaders Program](https://las.illinois.edu/resources/international/globallearning/leaders), I worked with Tijuana’s education department to support immigrant middle school students. 

To help bridge language barriers between students and faculty, I developed a free AI-powered translation web app that transcribes and translates live or recorded audio between English, Spanish, and Haitian Creole.



<br>
### Try the App!

*(If the Space is sleeping, click  "Restart Space" to wake it up!)*

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
  // Grab the iframe and your app's base URL
  const iframe = document.getElementById('gradio-app');
  const baseUrl = "https://yoyoyork-on-demand-spanish-translator.hf.space";
  
  // Function to check your site's theme and update the iframe
  function syncTheme() {
    const isDark = document.documentElement.getAttribute('data-theme') === 'dark';
    const targetUrl = isDark ? baseUrl + "/?__theme=dark" : baseUrl + "/?__theme=light";
    
    // Only reload the iframe if the URL actually needs to change
    if (iframe.src !== targetUrl) {
      iframe.src = targetUrl;
    }
  }

  // 1. Set the correct theme immediately when the page loads
  syncTheme();

  // 2. The Bulletproof Watcher: Stares directly at the HTML tag for theme changes
  const observer = new MutationObserver((mutations) => {
    mutations.forEach((mutation) => {
      if (mutation.attributeName === 'data-theme') {
        syncTheme();
      }
    });
  });

  // Start watching the <html> tag for attribute changes
  observer.observe(document.documentElement, { attributes: true });
</script>

---