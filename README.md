# SMART on FHIR Interactive Lab

### [Launch the Live Interactive Lab](https://burroclurse.github.io/SMART-on-FHIR-Interactive-Lab/)

An open-source, self-contained interactive learning workbench for mastering **SMART on FHIR Discovery (`/.well-known/smart-configuration`)**, **SMART v1/v2 Scopes**, **OAuth 2.0 with PKCE (`S256`)**, **Standalone vs. EHR Launch workflows**, and **OpenID Connect (`id_token`) vs. `access_token` vs. Patient Context**.

---

## What's Inside

The lab is organized as a suggested path for people new to SMART on FHIR. Every section keeps the full technical detail.

### 1. Start Here
* Plain-language orientation: John, his mother Eleanor, and who is involved in a SMART connection.
* How to read the lab: dark boxes are code, tinted text is an exact value, dotted words open the glossary.
* Four core concepts, each with a video, a summary, and a hands-on demo.

### 2. Guided Lab
* Opens on an overview of the big picture and the ten steps.
* Ten steps beside a live, searchable `/.well-known/smart-configuration` JSON inspector (`642` advertised scopes across `patient/`, `user/`, and `system/`).
* SMART v2 scope anatomy (`patient/Observation.rs` vs. `patient/Observation.cruds`), caregiver scenarios, a check after each step, and a 10-question final assessment.

### 3. Watch the Flow
* **6-Actor, 19-Step Sequence Diagram** (modeled after Epic's Standalone & EHR Launch architecture).
* **Standalone Launch (`launch-standalone`) vs. EHR Launch (`launch-ehr`)** toggle, **PKCE (`S256`) Tamper Tester**, and **Access Token Expiration + Refresh Token Renewal (`offline_access`)**.
* A build-it-yourself authorization URL builder.

### 4. Tokens (`id_token` vs. `access_token` vs. Context)
* Side-by-side comparison, the `fhirUser` claim, and a visual of `need_patient_banner`.

### 5. Go Deeper
* Collapsed reference sections, linked from the matching parts of the other tabs: vendor sandbox comparison (Epic, Oracle Health, mock server), wildcard vs. specific scopes, seven developer anti-patterns, a DevTools debugging guide, backend services (`client_credentials`), and seven error scenarios with fixes.

A searchable 123-term glossary opens from any page, including a Plain-Language Basics category for readers new to the technical words. The browser Back button returns to the previous tab.

---

## How to Run or Fork

This entire application is built in a **single, zero-build HTML file (`index.html`)** using React 18, Tailwind CSS, and Babel Standalone via CDN:

1. **Use Online:** Visit the [GitHub Pages live link](https://burroclurse.github.io/SMART-on-FHIR-Interactive-Lab/).
2. **Run Locally:** Clone or download this repository and double-click `index.html` in any modern web browser.
3. **Fork & Customize:** Click **Fork** in the top-right corner of GitHub, edit `index.html`, and enable GitHub Pages in your fork's settings.

---

## License

Released under the **MIT License** — free to use, modify, fork, and share for education and training.
