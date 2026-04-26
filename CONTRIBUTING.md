# Sådan bidrager du

Tak for din interesse! Denne ordbog lever af bidrag fra IT-folk og sprogfolk.

## Hvad kan du bidrage med?

- **Nye ord**: Et IT-udtryk der mangler i `data/terms.json`
- **Rettelser**: En klassifikation, oversættelse eller note der er forkert eller forældet
- **Eksempler**: Bedre eller flere eksempelsætninger
- **Kilder**: Links eller referencer der underbygger en klassifikation
- **Diskussion**: Åbn et issue hvis du er uenig i et eksisterende opslag

## Sådan gør du

1. **Fork** dette repo
2. **Opret en branch** med et beskrivende navn, fx `add-term-kubernetes` eller `fix-cloud-classification`
3. **Redigér** `data/terms.json` — hold filen sorteret alfabetisk efter `term_en`
4. **Sæt status** til `proposed` på nye eller ændrede opslag (eksisterende `approved`-opslag bevarer status indtil panelet har godkendt ændringen)
5. **Validér** at filen stadig er gyldig JSON og følger skemaet i `schema/terms.schema.json`
6. **Åbn en pull request** med en kort begrundelse

## Hvad gør et godt opslag?

- **Definitionen** er kort, neutral og på engelsk — ikke en lang afhandling
- **`note_da`** forklarer *hvorfor* udtrykket klassificeres som det gør, ikke bare hvad det betyder
- **Eksemplerne** er realistiske sætninger fra faktisk brug — ikke konstruerede skoleeksempler
- **Klassifikationen** er ærlig: hvis et udtryk faktisk bruges i begge former, så er det `coexists` — også selvom du personligt foretrækker den ene
- **Opslaget følger de redaktionelle principper** i [`PRINCIPLES.md`](PRINCIPLES.md) — bl.a. samskrivning af danske sammensætninger og afvisning af engelske grammatiske kalker

## Hvad gør et *dårligt* opslag?

- Personlige holdninger til *hvad det burde hedde* uden dokumentation for faktisk brug
- "Pure_loan" når Dansk Sprognævn eller udbredt fagsprog bruger noget andet
- Definitioner der i virkeligheden er reklametekst eller marketingsprog
- Eksempler hentet direkte fra én bestemt leverandørs dokumentation

## Beslutningsproces

Se [`GOVERNANCE.md`](GOVERNANCE.md). Kort fortalt: alle PR'er får en redaktionel gennemgang. Indtil panelet er etableret træffes beslutninger af repo-ejeren. Bagefter kræver godkendelse flertal i panelet.

## Kodeks

Vær respektfuld. Diskuter sprog og klassifikation, ikke personer. Det her er et fagligt projekt — uenighed er godt, men det skal være fagligt funderet.
