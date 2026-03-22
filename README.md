# Metavir 🦠

A daily-style virus taxonomy guessing game inspired by [Metazooa](https://metazooa.com). Identify the mystery virus in as few guesses as possible — each wrong guess reveals how your guess relates to the answer via a growing dendrogram.

**[Play it here →](https://donutbrew.github.io/metavir/)**

---

## How to play

- Type any virus name and pick from the autocomplete suggestions
- Each guess badge shows the **deepest taxonomic rank you share** with the mystery virus — click it to open the Wikipedia article for that taxon
- A **dendrogram** grows with each guess, mapping how your guesses branch away from the answer
- You have **21 guesses** to identify the virus
- Use **Show hint** for a one-line clue if you're stuck
- On a correct guess, an **electron micrograph or crystal structure image** is shown (linked externally with attribution), plus a **side-by-side comparison of all three classification systems**

---

## Taxonomy modes

Switch modes using the **5-rank / 8-rank / 15-rank** toggle in the header. Switching resets the current game.

| Mode | Ranks used | Based on |
|------|-----------|----------|
| **5-rank** | order → family → subfamily → genus | Classic pre-2017 ICTV system — the one most people learned |
| **8-rank** | realm → kingdom → phylum → class → order → family → genus | Simplified modern system (default) |
| **15-rank** | All populated ranks including subrealm, subphylum, subclass, suborder, subfamily, subgenus | Full current ICTV/NCBI standard |

The **win screen** shows all three systems side by side, designed to help people familiar with the classic system get oriented in the newer classification.

---

## Virus database

~60 viruses across major groups:

- **RNA viruses (Riboviria):** SARS-CoV-2, MERS-CoV, Influenza A/B, Ebola, Marburg, Rabies, Measles, Mumps, Nipah, Hendra, RSV, hMPV, Dengue, Zika, West Nile, Yellow fever, Hepatitis C, Poliovirus, Hepatitis A, Rhinovirus A, EV-D68, Norovirus, Chikungunya, Rubella, Hepatitis E, Lassa, Hantavirus, Rift Valley fever, CCHF, Rotavirus A, Tobacco mosaic virus
- **Retroviruses (Riboviria › Pararnavirae):** HIV-1, HIV-2, Hepatitis B, HTLV-1, Murine leukemia virus, Cauliflower mosaic virus
- **dsDNA viruses (Duplodnaviria):** HSV-1, HSV-2, VZV, CMV, EBV, KSHV, T4 phage, Lambda phage
- **Large DNA viruses (Varidnaviria):** Variola, Vaccinia, Mpox, Cowpox, Mimivirus, Pandoravirus, Adenovirus 5
- **ssDNA viruses (Monodnaviria):** HPV-16, HPV-18, BK polyomavirus, AAV2, Parvovirus B19
- **RNA phages:** MS2 bacteriophage

Taxonomy follows **NCBI/ICTV 2023–2024** classification.

---

## Micrograph image sources

Images are linked externally (not embedded) with full attribution:

- [UTMB Virus Images](https://www.utmb.edu/virusimages/the-virus-images) — educational use permitted
- [Texas DSHS Electron Micrographs](https://www.dshs.texas.gov/laboratory-services/programs-laboratories/microbiology-unit/viral-isolation/viral-isolation-electron-micrographs) — public domain
- [CDC Public Health Image Library (PHIL)](https://wwwn.cdc.gov/phil/) — public domain
- [NIAID](https://www.niaid.nih.gov/) — CC BY 2.0
- [Wikimedia Commons](https://commons.wikimedia.org/) — various open licenses (credited per image)

---

## Technical notes

- Single self-contained HTML file — no build step, no dependencies, no server required
- Fonts loaded from Google Fonts (Space Mono + DM Sans)
- Light/dark mode toggle
- Fully responsive

## Deployment

This site is hosted on **GitHub Pages** from the root of the `main` branch.

To deploy your own copy:
1. Fork this repo
2. Go to **Settings → Pages → Source: Deploy from branch → main / (root)**
3. Your copy will be live at `https://<your-username>.github.io/metavir/`

---

## Credits

Game concept inspired by [Metazooa](https://metazooa.com) by Trainwreck Labs.  
Virus taxonomy data from [NCBI Taxonomy Browser](https://www.ncbi.nlm.nih.gov/Taxonomy/Browser/wwwtax.cgi?id=10239) and the [ICTV](https://ictv.global/).  
