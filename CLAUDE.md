# CLAUDE.md – Instruksjoner for Claude (leses alltid først)

Dette er den primære instruksjonsfilen for prosjektet. Den skal leses ved oppstart av hver økt og følges til punkt og prikke.

---

## Grunnregler (skal aldri brytes)

1. **Aldri slett data.**
   - Rådata, mellomlagrede datasett og resultater skal alltid bevares.

2. **Aldri slett et program.**
   - Eksisterende skript og programmer skal aldri overskrives eller slettes.
   - Ved reorganisering eller erstatning: flytt det gamle programmet til `./legacy/` før det nye opprettes.
   - Mappestrukturen i `./legacy/` skal speile original plassering, slik at historikk er sporbar.

3. **Aldri forlat prosjektets rot.**
   - All aktivitet skal skje innenfor GDP-repoets rotmappe.
   - Bruk alltid relative stier fra roten.

---

## Regler for `./legacy/`

- `./legacy/` er arkivet for eldre versjoner av programmer og data.
- Filer flyttes hit (kopieres aldri bort uten at originalen er trygg).
- Behold original mappestruktur inne i `./legacy/` for sporbarhet.
- Eksempel: `./scripts/analyse.R` → `./legacy/scripts/analyse_v1.R`

---

## Nye regler

### Kontinuerlig git-lagring

- Etter hver meningsfull endring (nytt datasett, nytt skript, oppdatert fil) skal Claude automatisk kjøre `git add`, `git commit` og `git push`.
- Commit-meldinger skal være korte og beskrivende, på norsk.
- Formålet er at arbeid aldri går tapt – repoet på GitHub skal til enhver tid speile gjeldende tilstand.

---

### Fremdriftslogg – `./log/progress.md`

- Filen `./log/progress.md` er den løpende loggen over alt arbeid i prosjektet.
- Claude skal oppdatere denne filen **etter hver økt eller meningsfull endring**, med et nytt innlegg øverst.
- Innlegget skal inneholde:
  - Dato og klokkeslett (`YYYY-MM-DD HH:MM`)
  - Kort tittel på hva som ble gjort
  - Kulepunktliste over konkrete handlinger
  - Hvilke filer som ble påvirket
  - Eventuelle neste steg eller notater
- Formål: sikre at kontekst ikke går tapt ved avbrudd i chatten.

---

*Sist oppdatert: 2026-03-01 (lagt til regel om fremdriftslogg)*
