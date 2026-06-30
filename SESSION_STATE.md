# WEBICONS — SESIJOS BŪKLĖ (handoff)

**Data:** 2026-06-30 · **Projektas:** `C:\Users\Owner\Desktop\WEB kūrimas\webicons` (git repo)
**Statusas:** ✅ **GYVA INTERNETE** — `https://www.webicons.org`. Visa medžiaga commit'inta (`main`, commit `e69ef1f`), GitHub repo sukurtas ir kodas įkeltas.

> ⚠️ **Kas tai per projektas:** **angliška, tarptautinė versija** WEBU STUDIJA dizaino — vienas statinis `index.html` su inline `<style>` + inline `<script>`. Tas pats soft-UI neumorfinis dizainas, Three.js gaublys, bet brandas **WEBICONS** ir tekstai/SEO/structured data — angliški. **NĖRA** Tailwind/React/build žingsnio.

---

## 🚀 DEPLOY — PADARYTA (gyva)
- **Domenas:** `webicons.org` (pirktas per Hostinger). **`www.webicons.org` = pagrindinis (canonical)**, `webicons.org` (be www) irgi veikia ir ves į tą pačią svetainę.
- **DNS Hostinger'yje:** `A @ → 76.76.21.21`, `CNAME www → cname.vercel-dns.com`. Nameserveriai NEKEISTI. `MX`/`TXT`/DKIM įrašai (paštui) **nepaliesti**.
- **Hostingas:** Vercel, projektas **`webicons`** (team `agnyte16`, org `team_qCPQvdp0BPyAo7CRQxC1FY7Y`). `webicons/.vercel/project.json` susietas (`prj_I7M4Nbh1jcTFaxo5ybq9XOTwsHeA`).
- **Kaip iš naujo deploy'inti (rankiniu būdu):**
  ```
  vercel deploy "C:\Users\Owner\Desktop\WEB kūrimas\webicons" --prod --yes --token <TOKEN_iš_agnyte16>
  ```
- ⚠️ **Auto-deploy iš GitHub — NEUŽBAIGTA.** `vercel git connect` nepavyko, nes **Vercel GitHub App niekada nebuvo įdiegtas** `agnyte16` paskyroje (visi deploy'ai ėjo per CLI token). **Reikia:** vartotoja eina į `https://github.com/apps/vercel` → Install → pasirenka `agnyte16` → Repository access → prideda `webicons` (ir/ar `webu-studija`) → Save. Tada AŠ baigsiu `vercel git connect`, kad push į `main` automatiškai deploy'intų.

---

## 🤝 GITHUB HANDOFF (kolegai) — kvietimas IŠSIŲSTAS, dar NEPRIIMTAS
- **Repo:** `https://github.com/agnyte16/webicons` — **PRIVATUS**, `main` = default šaka, 23 failai (commit `e69ef1f`).
- **Kolega:** GitHub `pakammakam11-boop` (el. paštas `pakammakam11@gmail.com`) — **tas pats kolega**, kuris dirba su WEBU STUDIJA. Pakviestas **collaborator'iu su `write` (push)** teisėmis per API (`gh api -X PUT repos/agnyte16/webicons/collaborators/pakammakam11-boop -f permission=push`).
- **STATUSAS (2026-06-30 ~22:32):** kvietimas **`pending`** (matomas per `gh api repos/agnyte16/webicons/invitations`) — kolega DAR NEPRIĖMĖ. Kol nepriėmė, `https://github.com/agnyte16/webicons` jam (ir bet kam neprisijungus tinkama paskyra) rodo **404 „This is not the web page..."** — tai NORMALU privačiam repo, NE klaida.
- **Sprendimas kolegai:** nusiųsti TIKSLIAI šitą linką (ne paprastą repo linką): **`https://github.com/agnyte16/webicons/invitations`** → jis turi būti prisijungęs prie SAVO `pakammakam11-boop` paskyros → paspausti „Accept invitation".
- **Patikrinti vėliau:** `gh api repos/agnyte16/webicons/collaborators/pakammakam11-boop` → jei grąžina 200 (ne 404) = priėmė.

---

## 📨 PAŠTAS / FORMA / BOOKING — viskas veikia (patikrinta)
- **Paštas:** `info@webicons.org` (sukurtas per Hostinger Webmail).
- **Kontaktų forma:** `formsubmit.co/ajax/info@webicons.org` (AJAX, be backend'o). **Aktyvuota ir PATIKRINTA realiu testiniu siuntimu** — `{"success":"true"}`, laiškas atkeliavo į `info@webicons.org`. Honeypot laukas `_honey` (ne `botcheck` kaip WEBU STUDIJA versijoje).
- **Konsultacijų booking:** `https://cal.eu/webicons/30-min-consultation` (Cal.eu, „For myself" event type, savininkas „Paul Matthew" — kolega, įkūrėjas/vadovas). Įdėtas 2 vietose (`.cta` hero + footer „Book a call"). ⚠️ **Nepatikrinta**, ar Cal.eu pranešimai eina į `info@webicons.org` — reikėtų patikrinti Cal.eu Settings.

---

## Skirtumai nuo WEBU STUDIJA (originalo, iš kurio nukopijuota)
- Kalba: **EN** (`lang="en"`), visas tekstas/SEO/OG/Twitter/JSON-LD perrašytas angliškai.
- Brand: **WEBICONS** (ne WEBU STUDIJA), domenas `webicons.org` (ne `.lt`).
- Pašalinta kolegos asmeninė info: Google Ads gtag (`AW-18226540442`), `paulius.jpg`, LinkedIn, telefonas.
- Gaublio projektai sutrumpinti iki **10** (turimi lokalūs screenshot'ai; originale buvo 13).
- Kainos/pricing struktūra identiška (€499/€599/€599/€999 + B2B custom).
- **Brand ikona/logo sukurta atskirai** (žr. žemiau).

## 🎨 Brand ikona (sukurta 2026-06-29)
`C:\Users\Owner\Desktop\WEB kūrimas\webicons-icon\` — soft-UI tamsus ženklas (salotinis švytintis rombas 45° + „WEBICONS" + „WEB DESIGN STUDIO"), 1024×1024:
- `webicons-icon.png` / `.jpg` — pilnas tamsus variantas (savarankiškas, dėti ant bet kokios nuotraukos).
- `webicons-icon-transparent.png` — permatomas baltas variantas (kai norisi matyti foną pro šalį).
- `.svg` šaltiniai abiems — redaguojami.
- **NE susieta su svetainės og:image** — `img/og-cover.jpg` svetainei vis dar trūksta (žr. pending).

---

## Pending / flag'ai
1. **Auto-deploy GitHub→Vercel** — žr. aukščiau, laukia vartotojos `github.com/apps/vercel` instaliacijos.
2. **Kolegos GitHub kvietimas** — laukia priėmimo (`/invitations`).
3. **Cal.eu pranešimų el. paštas** — nepatikrinta, ar eina į `info@webicons.org`.
4. **`og-cover.jpg`** (1200×630 social share) — vis dar nėra; `webicons-icon` aplankas galėtų būti pagrindas.
5. **Web3Forms raktas** ankstesnėje iteracijoje buvo placeholder'is — **PAKEISTA į FormSubmit**, Web3Forms nebenaudojamas šitam projektui.

## Resume cheatsheet
```
cd "C:/Users/Owner/Desktop/WEB kūrimas/webicons"
git log --oneline                 # e69ef1f (main)
git remote -v                     # origin = github.com/agnyte16/webicons
# deploy: vercel deploy --prod --yes --token <agnyte16_token>   (iš webicons/)
# GitHub token: Windows Credential Manager, target "GitHub - https://api.github.com/agnyte16"
#   (CredRead P/Invoke patternas — žr. WEBU STUDIJA SESSION_STATE.md jei reikia pavyzdžio)
```
