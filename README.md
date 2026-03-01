# GDP – Bruttonasjonalprodukt

Prosjekt for innhenting, bearbeiding og analyse av BNP-data.

---

## Repostruktur

```
GDP/
├── README.md          # Denne filen – oversikt over repoet
├── CLAUDE.md          # Instruksjoner til Claude (leses alltid først)
│
├── data/
│   ├── raw/           # Ubehandlede rådata (aldri endre disse)
│   └── processed/     # Rensede og bearbeidede datasett
│
├── scripts/           # Programmer og skript for analyse
│
├── output/            # Resultater, tabeller og figurer
│
└── legacy/            # Arkiv for eldre versjoner av programmer og data
```

> Strukturen utvides etter hvert som prosjektet vokser. README oppdateres fortløpende.

---

## Viktig å vite

### For fremtidige versjoner av deg selv (og Claude!)

- **Les `CLAUDE.md` først.** Den inneholder regler som alltid gjelder.
- **Data slettes aldri.** Rådata i `data/raw/` er hellig – de skal aldri endres eller slettes.
- **Programmer slettes aldri.** Gamle versjoner arkiveres i `./legacy/` med original mappestruktur bevart.
- **Jobb alltid fra rotmappen** (GDP/). Bruk relative stier.

### Datakilder

*(Legg til datakilder her etter hvert som de tas i bruk, f.eks. SSB, Verdensbanken, IMF, FRED osv.)*

### Metode og analyser

*(Beskriv hvilke analyser som gjøres, hvilke variable som brukes, og hva resultatene skal brukes til.)*

---

## Endringslogg

| Dato       | Endring                          |
|------------|----------------------------------|
| 2026-03-01 | Initiell oppsett av repo         |

---

*Prosjekteier: eal024*
