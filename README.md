# SMART on FHIR Interactive Lab

### [Open the lab](https://burroclurse.github.io/SMART-on-FHIR-Interactive-Discovery-OAuth-2.0-Lab/)

How a health app finds a server, asks permission, and gets its tokens. A free, hands-on lab for people new to **SMART on FHIR**: discovery (`/.well-known/smart-configuration`), SMART v1/v2 scopes, OAuth 2.0 with PKCE (`S256`), standalone vs. EHR launch, and `id_token` vs. `access_token` vs. patient context.

Everything follows one story: John connects a graphing app to his mother Eleanor's lab results.

---

## The five tabs

The tabs are a suggested path. Each one builds on the last.

### 1. Start Here
* Who is involved in a SMART connection, in plain words.
* How to read the lab: dark boxes are code, tinted text is an exact value, dotted words open the glossary.
* Four core concepts, each with a video, a plain-language summary, key takeaways and a hands-on demo.

### 2. Guided Lab
* Opens on an overview: the big picture, the ten steps, and how each step works.
* Ten steps beside a real server's settings file, with the lines each step is about highlighted. The file is searchable and lists `642` advertised scopes across `patient/`, `user/` and `system/`.
* Scope anatomy (`patient/Observation.rs` vs. `patient/Observation.cruds`), a caregiver scenario, a check after several steps, and a 10-question final assessment.

### 3. Watch the Flow
* The whole sign-in, one message at a time: six parties and nineteen messages, modeled on Epic's published launch diagrams.
* Standalone launch vs. EHR launch, stepped through in four phases with the exact request and response for each.
* Try to break it: tamper with PKCE, let the access token expire and renew it with a refresh token (`offline_access`), or send the wrong token.
* Build the sign-in URL yourself.

### 4. Tokens
* `id_token` vs. `access_token` vs. patient context, side by side.
* The `fhirUser` claim and a visual of `need_patient_banner`.

### 5. Go Deeper
Reference sections, collapsed until opened. The other four tabs link straight to the matching section.
* Try a real SMART launch against a free public test server.
* Compare vendor sandboxes (Epic, Oracle Health, a mock server).
* Wildcard vs. specific scopes, granular scopes, and USCDI / US Core.
* Seven common developer mistakes, a browser DevTools debugging guide, and seven error scenarios with fixes.
* Backend services (`client_credentials`) and bulk data export (`$export`).

### Throughout
* A searchable 123-term glossary, opened from the **Glossary** button or any dotted word. Its "Plain-Language Basics" category covers everyday terms like sandbox and endpoint.
* Anything you can press looks like a raised button.
* The browser's Back button returns to the previous tab. Each tab has its own address (for example `#guided-lab`), so a link can open the lab on a given tab.
* Progress is saved in your browser, so a refresh picks up where you left off.

---

## Run it or fork it

The whole lab is one HTML file (`index.html`) with no build step. It loads React 18, Tailwind CSS and Babel Standalone from a CDN.

1. **Online:** open the [live lab](https://burroclurse.github.io/SMART-on-FHIR-Interactive-Discovery-OAuth-2.0-Lab/).
2. **On your computer:** download `index.html` (or use the download button at the bottom of the lab) and open it in any modern browser.
3. **Your own copy:** click **Fork** on GitHub, edit `index.html`, and turn on GitHub Pages in your fork's settings.

---

## License

MIT License. Free to use, change, fork and share for education and training.
