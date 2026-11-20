# Framework Consent Mode v2 & Conformidade LGPD | TAVARDT Brasil

[![Privacy Compliance](https://img.shields.io/badge/Compliance-Consent%20Mode%20v2-5b3cf5.svg)](https://tools.tavardt.com/br/)
[![Regulatory Standard](https://img.shields.io/badge/Region-BRL-00C853.svg)](https://ag.tavardt.com/br/)

Implementação técnica do Google Consent Mode v2, bloqueio prévio de scripts e conformidade com a LGPD e ANPD no Brasil.

Maintained by the analytics, privacy engineering, and cybersecurity division at [TAVARDT Brasil](https://ag.tavardt.com/br/).

---

## 1. Architecture & Execution Order

To achieve full compliance with Lei Geral de Proteção de Dados (LGPD) e Diretrizes ANPD, this snippet must be positioned in the `<head>` of your website **immediately before** your Google Tag Manager container or tracking loader:

```html
<script src="consent-mode-v2.js"></script>
<!-- Google Tag Manager / Analytics Script Follows Here -->
```

---

## 2. Core Capabilities

* **Strict Default 'Denied' Posture:** Enforces privacy by default across all advertising, telemetry, and personal identifier parameters.
* **Consent Update API:** Provides an event-driven `window.tavardtUpdateConsent()` method that triggers a structured `tavardt_consent_updated` dataLayer event.
* **Ads Data Redaction:** Automatically strips click identifiers (such as GCLID and DCLID) from ad requests when marketing consent is absent.
* **URL Passthrough:** Preserves conversion attribution across domain boundaries using cryptographic hashes without storing persistent browser cookies.

---

## 3. Compliance Documentation

Review our jurisdictional implementation guidelines:

* [Technical Checklist](checklist.md): Step-by-step audit points for tag governance under Lei Geral de Proteção de Dados (LGPD) e Diretrizes ANPD.

---

## 4. Online Diagnostic Suite

Audit your public web applications and verify tracking privacy on our regional testing platform:

* [Online HTTP Security Headers Checker](https://tools.tavardt.com/br/security-headers-check/)
* [Exposed Credentials Scanner](https://tools.tavardt.com/br/exposed-files-scanner/)
* [DMARC & Anti-Spoofing Verifier](https://tools.tavardt.com/br/dmarc-checker/)
* [Complete Regional Diagnostic Suite](https://tools.tavardt.com/br/)

For comprehensive conversion tracking audits, consent management implementation, and technical consulting, contact [TAVARDT Brasil](https://ag.tavardt.com/br/contact/).
