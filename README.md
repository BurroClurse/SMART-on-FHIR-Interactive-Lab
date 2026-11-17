# SMART on FHIR Interactive Lab

### [Launch the Live Interactive Lab](https://burroclurse.github.io/SMART-on-FHIR-Interactive-Lab/)

An open-source, self-contained interactive learning workbench for mastering **SMART on FHIR Discovery (`/.well-known/smart-configuration`)**, **SMART v1/v2 Scopes**, **OAuth 2.0 with PKCE (`S256`)**, **Standalone vs. EHR Launch workflows**, and **OpenID Connect (`id_token`) vs. `access_token` vs. Patient Context**.

---

## What's Inside

### 1. 10-Step Guided Discovery & Scopes Lab
* Interactive walkthrough paired with a live, searchable `/.well-known/smart-configuration` JSON inspector (`642` advertised scopes across `patient/`, `user/`, and `system/`).
* Interactive SMART v2 scope anatomy decoder (`patient/Observation.rs` vs. `patient/Observation.cruds`) and caregiver proxy scenarios.
* Opens on an overview of the ten steps, with quick checks along the way and a 10-question final assessment.

### 2. Core Concepts & Video Hub
* A plain-language start that follows John and his mother Eleanor.
* Visual sandboxes comparing open public FHIR servers (HAPI) vs. protected PHI servers, scope narrowing rules, token roles, and Epic / Oracle Health launch flowcharts.

### 3. Interactive OAuth 2.0, PKCE & Refresh Token Simulator
* **6-Actor, 19-Step Sequence Diagram** (modeled after Epic's Standalone & EHR Launch architecture).
* **Standalone Launch (`launch-standalone`) vs. EHR Launch (`launch-ehr`)** toggle showing how `launch` context tokens, `encounter`, `need_patient_banner`, and `fhirUser` change on the wire.
* **PKCE (`S256`) Tamper Tester** and **Access Token Expiration + Refresh Token Renewal (`offline_access`)** simulator.

### 4. Token Deep-Dive Lab (`id_token` vs. `access_token` vs. Context)
* Side-by-side comparison matrix, 3-part JWT decoder (`Header.Payload.Signature`), and interactive security boundary checks.

### 5. Go Deeper Reference
* Collapsed sections on vendor sandboxes, wildcard and granular scopes, USCDI and US Core, developer mistakes, DevTools debugging, backend services, bulk export, and error scenarios. The other sections link straight to them.

A searchable 123-term glossary opens from anywhere, with a Plain-Language Basics category for new readers.

---

## How to Run or Fork

This entire application is built in a **single, zero-build HTML file (`index.html`)** using React 18, Tailwind CSS, and Babel Standalone via CDN:

1. **Use Online:** Visit the [GitHub Pages live link](https://burroclurse.github.io/SMART-on-FHIR-Interactive-Lab/).
2. **Run Locally:** Clone or download this repository and double-click `index.html` in any modern web browser.
3. **Fork & Customize:** Click **Fork** in the top-right corner of GitHub, edit `index.html`, and enable GitHub Pages in your fork's settings.

---

## License

Released under the **MIT License** — free to use, modify, fork, and share for education and training.
