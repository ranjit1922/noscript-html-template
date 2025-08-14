---

# noscript-html-template

A lightweight HTML template that provides a fallback message and instructions for users with JavaScript disabled.

## Usage Steps

### 1. Add the `noscript` class and script to remove it

Place this at the very start of your HTML document:

```html
<!DOCTYPE html>
<html lang="en" class="noscript" itemscope itemtype="http://schema.org/WebPage">
<head>
<script>
  document.documentElement.classList.remove('noscript');
</script>

This ensures that when JavaScript is enabled, the noscript class is removed from the <html> element.

2. Add the <noscript> fallback

Place this block at the end of your <head> or start of your <body>:

<noscript>
  <div id="noscript-frame-wrapper">
    <a href="https://ranjit1922.github.io/noscript-html-template" target="_blank" rel="noopener" id="noscript-link">
      JavaScript is disabled. Click here for help.
    </a>
    <iframe
      src="https://ranjit1922.github.io/noscript-html-template"
      title="JavaScript Disabled Instructions"
      loading="lazy"
      sandbox="allow-same-origin"
      crossorigin="anonymous"
      fetchpriority="high">
    </iframe>
  </div>
</noscript>

This gives the user a friendly notice plus an embedded guide when JavaScript is disabled.

3. Style the fallback (optional)

Include CSS to make the noscript content stand out and match your design:

.noscript #noscript-frame-wrapper {
  display: block;
  padding: 1rem;
  background: #fff3cd;
  border: 1px solid #ffeeba;
  color: #856404;
}

4. Deployment

Once integrated, deploy your site as usual. The noscript fallback will appear selectively for users without JavaScript.


---

Demo: Live Example

License: Apache License 2.0

---

No fuss copying — just paste this over your existing REMADE.md (or better, rename to `README.md`), and it’s good to go.

Let me know if you want someone to tick through the Apache header text or any legal boilerplate, or keep it lean and focused like this.0

