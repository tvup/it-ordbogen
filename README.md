# it-ordbogen

## IT-ordbog: Engelsk → Dansk

> *Hvad siges i dansk tale, og hvad skrives på dansk?*

En åben ordbog over IT-udtryk fra handels-engelsk med deres danske modstykker — uanset om de ender som rene låneord, tilpassede låneord eller får en egentlig dansk oversættelse.

## Formål

Når man arbejder i IT-branchen i Danmark, støder man konstant på engelske udtryk. Nogle bliver brugt som rene låneord (*deployment*, *pipeline*), andre tilpasses dansk udtale eller bøjning (*at deploye*, *en pipeline*), og andre igen har eller får danske oversættelser (*cloud* → *sky*, *reboot* → *genstart*). Denne ordbog dokumenterer den faktiske sprogbrug og giver et fagligt funderet bud på hvad et udtryk hedder på dansk.

## Datakilde

Alle ord findes i [`data/terms.json`](data/terms.json). En post ser sådan ud:

```json
{
  "term_en": "harddisk",
  "term_da": "harddisk",
  "loanword": "adapted_loan",
  "definition_en": "A non-volatile data storage device using rotating magnetic platters.",
  "note_da": "Bruges som låneord med dansk bøjning: 'en harddisk', 'harddisken', 'flere harddiske'.",
  "alternatives_da": [],
  "rejected_translations_da": [
    {
      "term": "fastpladelager",
      "reason": "Foreslået som dansk fagterm, men har aldrig fundet udbredt anvendelse — hverken i daglig tale eller i IT-fagsprog."
    }
  ],
  "examples": [
    "Harddisken er ved at være fyldt op.",
    "Vi udskifter de gamle harddiske med SSD'er."
  ],
  "category": "hardware",
  "status": "approved"
}
```

### Felter

| Felt | Beskrivelse |
|---|---|
| `term_en` | Det engelske udtryk (lowercase, medmindre det er et egennavn) |
| `term_da` | Det danske udtryk som det typisk skrives — kan være identisk med `term_en` ved låneord |
| `loanword` | Klassifikation, se nedenfor |
| `definition_en` | Kort, neutral definition på engelsk |
| `note_da` | Kommentar på dansk om brug, bøjning, register, osv. |
| `alternatives_da` | Liste af danske alternativer der findes i brug, men som ikke er primærvalg |
| `rejected_translations_da` | Foreslåede oversættelser der *ikke* er accepteret — hver med en `reason` der dokumenterer hvorfor (fx manglende udbredelse, misvisende, kun i ældre opslagsværker) |
| `examples` | Eksempelsætninger der viser udtrykket i naturlig brug |
| `category` | Fagligt område, fx `devops`, `security`, `networking`, `data`, `frontend`, `general` |
| `status` | `approved`, `proposed`, `under_review`, `disputed` |

### Klassifikation af låneord

| Værdi | Betydning |
|---|---|
| `pure_loan` | Bruges uændret på dansk (*pipeline*, *deployment*) |
| `adapted_loan` | Låneord med dansk bøjning eller stavning (*at deploye*, *en server*) |
| `translated` | Har en etableret dansk oversættelse der primært bruges (*reboot* → *genstart*) |
| `coexists` | Både låneord og dansk oversættelse er i udbredt brug (*cloud* / *sky*) |
| `calque` | Direkte oversættelseslån, ord-for-ord (*motherboard* → *bundkort*) |

## Hvordan bidrager man?

1. Fork repoet
2. Tilføj eller redigér en post i `data/terms.json`
3. Sæt `status: "proposed"` på nye eller ændrede poster
4. Åbn en PR med kort begrundelse — gerne med kilder til faktisk sprogbrug

Se [`CONTRIBUTING.md`](CONTRIBUTING.md) for detaljer.

## Beslutningsproces

Ordbogen er åben for bidrag, men beslutninger om hvad der ender som godkendt indhold (`status: "approved"`) træffes af et **fagligt panel**.

- **Indtil panelet er etableret**: Beslutninger træffes af repo-ejeren ([@tvup](https://github.com/tvup)).
- **Når panelet er på plads**: Se [`GOVERNANCE.md`](GOVERNANCE.md) for sammensætning, afstemningsregler og hvordan man bliver panelmedlem.

Princippet er **demokrati med respekt for faglighed**: alle kan foreslå og diskutere, men den endelige redaktionelle beslutning ligger hos folk med dokumenteret IT-faglig og/eller sproglig baggrund.

## Licens

- **Indhold** (ordbogsdata, definitioner, noter): [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
- **Kode** (scripts, evt. UI): [MIT](LICENSE-CODE)

Se [`LICENSE`](LICENSE) for indhold og [`LICENSE-CODE`](LICENSE-CODE) for kode.
