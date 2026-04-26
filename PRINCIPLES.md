# Redaktionelle principper

Disse principper styrer **hvad ordbogen optager og hvordan vi klassificerer**. De er redaktionelle, ikke rent deskriptive: vi beskriver dansk IT-sprog, men vi tager også stilling til hvad der hører hjemme i ordbogen og hvad der ikke gør.

## 1. Sproglige strukturer ændres ikke

Engelske grammatiske bestanddele — suffikser, partikler, afledninger — accepteres ikke som danske IT-udtryk. Et IT-udtryk er et fagligt indhold; det er ikke en sproglig konstruktion eller en stilfigur.

**Eksempel der ikke optages:**

> *"Vi mødes kl. 14-ish."*

`-ish` er et engelsk afledningssuffiks, ikke et IT-udtryk og ikke et låneord. Det er en sproglig deformation, ikke en faglig term. Det samme gælder partikler og modale tilføjelser som *kind of*, *sort of*, *literally*, samt grammatiske kalker af typen "X-vis" hvor *-vis* gøres til frit mode-suffiks.

**Undtagelse:** hvis suffikset indgår fast i et navne- eller udsagnsord der reelt bruges som låneord — fx *deployment*, *deployer*, *deployede* — optages **det fulde udtryk** som låneord. Det er ord, ikke løse suffikser, ordbogen tager stilling til.

## 2. Sammensatte ord skrives sammen efter danske regler

Når engelske flerords-udtryk får et dansk modstykke, skrives det danske sammen efter dansk retskrivning. Særskrivning er én af de mest udbredte fejl i dansk IT-sprog, og ordbogen skal ikke kanonisere den.

| Engelsk | Dansk (rigtig) | Dansk (forkert) |
|---|---|---|
| version conflict | versionskonflikt | version konflikt |
| backup strategy | backupstrategi | backup strategi |
| cloud provider | cloududbyder | cloud udbyder |
| log file | logfil | log fil |
| build pipeline | build-pipeline / buildpipeline | build pipeline |

**Praktiske regler:**

- **Sammensætning på dansk** følger dansk retskrivning — uanset om grundordene er danske eller låneord. *Backupstrategi*, ikke *backup strategi*.
- **Bindestreg** kan tillades i overgangssammensætninger der indeholder et fremmedord eller en flerordsbestanddel (*cloud-native*, *open source-projekt*, *build-pipeline*), især hvis sammenskrivning gør udtrykket svært at læse.
- **Særskrivning** (to ord med mellemrum) er ikke tilladt i poster der optages som `approved`.
- Ved tvivl konsulteres Dansk Sprognævn / Retskrivningsordbogen.

## 3. Hvor reglerne passer ind i datamodellen

Når en post afvises på baggrund af én af disse principper, skal det dokumenteres:

- **Afvist oversættelsesforslag** (fx *version konflikt* med mellemrum) skrives ind under `rejected_translations_da` med begrundelse, der eksplicit henviser til princippet (fx *"Særskrivning af dansk sammensætning, jf. PRINCIPLES.md §2"*).
- **Afvist optagelse** (fx hele *14-ish*-eksemplet) optages **ikke** som post — det er ikke et IT-udtryk overhovedet. Hvis spørgsmålet kommer op i en PR, lukkes den med henvisning til §1.

---

Listen er ikke udtømmende. Flere principper kan tilføjes via PR efter samme proces som andre governance-ændringer (se [`GOVERNANCE.md`](GOVERNANCE.md)).
