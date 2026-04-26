# Redaktionelle principper

Disse principper styrer **hvad ordbogen optager og hvordan vi klassificerer**. De er redaktionelle, ikke rent deskriptive: vi beskriver dansk IT-sprog, men vi tager også stilling til hvad der hører hjemme i ordbogen og hvad der ikke gør.

## 1. Sproglige strukturer ændres ikke

Engelske grammatiske bestanddele — suffikser, partikler, afledninger — accepteres ikke som danske IT-udtryk, **heller ikke når de hægtes på et ord der i sig selv er en IT-term**. Et IT-udtryk er et fagligt indhold; det er ikke en sproglig konstruktion eller en stilfigur.

**Eksempel der ikke optages:**

> *"Vi skal nok basere det på noget token-ish i stedet."*

Her er *token* en regulær IT-term og hører hjemme i ordbogen som selvstændigt opslag. Men *-ish* er en engelsk approksimations-suffiks ("noget der minder om") som her er gjort til frit mode-suffiks i dansk syntaks. Det er ikke *token* der er problemet — det er det engelske grammatiske mønster der pålægges dansk. Sådanne konstruktioner afvises uanset om grundordet er et IT-udtryk eller ej; ordbogen tager stilling til ord og udtryk, ikke til grammatiske kalker.

Tilsvarende afvises partikler og modale tilføjelser som *kind of*, *sort of*, *literally* brugt på dansk, samt frit dannede afledninger der efterligner engelske mønstre.

**Undtagelse:** hvis suffikset indgår fast i et navne- eller udsagnsord der reelt bruges som låneord — fx *deployment*, *deployer*, *deployede* — optages **det fulde udtryk** som låneord. Det er etablerede ord, ikke løse suffikser, ordbogen tager stilling til.

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
- **Særskrivning** (to ord med mellemrum) er ikke tilladt i opslag der optages som `approved`.
- Ved tvivl konsulteres Dansk Sprognævn / Retskrivningsordbogen.

## 3. Hvor reglerne passer ind i datamodellen

Når et opslag afvises på baggrund af én af disse principper, skal det dokumenteres:

- **Afvist oversættelsesforslag** (fx *version konflikt* med mellemrum) skrives ind under `rejected_translations_da` med begrundelse, der eksplicit henviser til princippet (fx *"Særskrivning af dansk sammensætning, jf. PRINCIPLES.md §2"*).
- **Afvist optagelse** (fx *token-ish*-konstruktionen) optages **ikke** som selvstændigt opslag — den grammatiske kalke er ikke et IT-udtryk, selv når grundordet er det. Hvis spørgsmålet kommer op i en PR, lukkes den med henvisning til §1.

---

Listen er ikke udtømmende. Flere principper kan tilføjes via PR efter samme proces som andre governance-ændringer (se [`GOVERNANCE.md`](GOVERNANCE.md)).
