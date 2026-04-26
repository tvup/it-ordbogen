# Beslutningsproces (Governance)

Princippet er **demokrati med stor respekt for faglighed**. Alle kan foreslå, alle kan diskutere, men endelige beslutninger træffes af folk med dokumenteret IT-faglig og/eller sproglig baggrund.

## Faser

### Fase 1: Solo-redaktion (nu)

Indtil panelet er etableret, træffer repo-ejeren ([@tvup](https://github.com/tvup)) alle beslutninger. PR'er bliver stadig diskuteret offentligt, men endelig godkendelse ligger hos én person.

Mål: Få nok kvalitetsindhold og bidragydere til at det giver mening at samle et panel.

### Fase 2: Etablering af panel

Når repoet har:

- Mindst 100 godkendte poster
- Mindst 5 aktive bidragydere med substantielle PR'er
- Mindst én sprogfagligt kvalificeret bidragyder

…udvides redaktionen til et panel på 3–7 personer.

### Fase 3: Panel-redaktion

Panelet træffer beslutninger ved simpelt flertal blandt aktive medlemmer. Ved stemmelighed har panelets formand (oprindeligt repo-ejeren) den afgørende stemme.

## Sammensætning af panelet

Panelet skal balancere:

- **IT-faglighed**: Mindst halvdelen af medlemmerne skal have erhvervserfaring fra IT-branchen (udvikler, arkitekt, sysadmin, sikkerhedsfaglig, datafaglig osv.)
- **Sproglig faglighed**: Mindst ét medlem med dokumenteret sprogfaglig baggrund (cand.mag. i dansk, oversætter, sprognævnstilknytning eller tilsvarende)
- **Bredde**: Forskellige fagområder repræsenteret — undgå at hele panelet kommer fra fx kun frontend eller kun infra

## Hvordan bliver man medlem?

1. Bidrag løbende med kvalitets-PR'er over mindst 3 måneder
2. Vis at du kan diskutere fagligt og acceptere beslutninger du ikke selv stemte for
3. Bliv nomineret af et eksisterende panelmedlem, eller selv ansøg via et issue mærket `panel-application`
4. Bliv godkendt af et flertal i panelet

## Hvad bestemmer panelet om?

- Status-skift: `proposed` → `approved`, eller `approved` → `disputed`
- Klassifikation af låneord ved uenighed
- Tilføjelse/fjernelse af kategorier
- Ændringer i skemaet (`schema/terms.schema.json`)
- Ændringer i denne governance-fil

## Hvad bestemmer panelet *ikke* om?

- Kode (scripts, evt. UI) — det styres som almindelig open source af maintainere
- Repoets infrastruktur (hosting, CI, navngivning af repo)
- Licensvalg (kræver enstemmighed eller bred høring)

## Konflikter

Hvis et panelmedlem konsekvent ikke accepterer flertalsbeslutninger, eller agerer i strid med kodeks, kan medlemmet ekskluderes ved 2/3-flertal i panelet.

## Ændringer til denne fil

Ændringer kræver flertal i panelet. I solo-fasen kræver de en eksplicit PR med mindst 14 dages åbent kommentarvindue.
