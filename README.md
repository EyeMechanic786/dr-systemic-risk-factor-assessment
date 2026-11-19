# DR Systemic Risk Factor Assessment tool

Local clinical decision support for systemic risk factors in diabetic retinopathy and diabetic macular oedema. It is a single page that runs in a browser on a clinic workstation, iPhone, or Android phone. It is not an app-store product.

No assessment data leaves the device. Cases stay in the browser tab until it is closed. Use anonymised QI study IDs unless the Excel file is saved to an encrypted NHS Trust network drive.

Confirm every alert against current NICE guidance, QOF, and local protocol before acting.

## Open it

Any current browser can open the tool at:

**https://eyemechanic786.github.io/dr-systemic-risk-factor-assessment/**

That address works on a clinic PC, another laptop, and a mobile phone. The page is public so no GitHub sign-in is required. Entered cases stay in that browser and are not uploaded.

A wide screen uses the clinic layout. A phone uses one scrolling page. You can still open `index.html` directly from a saved copy of this folder.

On a phone, after the page has loaded, use **Add to Home Screen**:

- iPhone: Safari Share button, then Add to Home Screen.
- Android: Chrome menu, then Add to Home screen or Install app.

The phone view is one scrolling page. After it is added to the home screen, later visits can open from the icon. `manifest.webmanifest`, `sw.js`, and the icon files support that home-screen use.

## What you record

The page covers ocular grade for each eye, metabolic and cardio-renal measures, lifestyle and neuropathy, diabetic foot status including amputation, current UK BNF medicines used in this clinic (with GLP-1 and dual GIP/GLP-1 set out separately), and any other disease by ICD-10 search or free text.

Alerts, the EPR summary, and the GP letter update as you enter data. Copy buttons place the EPR summary or the GP paragraph on the clipboard.

## Audit export

**Log Case to Session** stores the case in the open tab. The same QI ID updates that case and keeps its number. A blank QI ID is a new case. Numbers run 1, 2, 3 in the order cases were first logged.

**Export Audit Excel** downloads `retina_qi_systemic_audit_YYYY-MM-DD.xlsx` with two sheets:

- **Full audit** — every recorded field, with `case_no` first.
- **Simple** — a shorter sheet for day-to-day review, including both eyes, key medicines, foot status, other disease, red and amber counts, and QOF codes.

Clear Form empties the entry screen and leaves the logged session in place.
