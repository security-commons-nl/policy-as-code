# policy-as-code

Beleid als code: regels die je kunt draaien in plaats van alleen lezen.

Status: concept. Idee en denkrichtingen; geen werkende tool.

**Status: concept (idee).** Nog geen werkende tool; dit is een uitnodiging om mee te denken.

## Voor wie

CISO's en ISO's die beleid toetsbaar willen maken.

## Snel starten

Er is nog niets te draaien. Lees het idee hieronder en denk mee via een issue.

## Bijdragen

Zie de [CONTRIBUTING](https://github.com/security-commons-nl/.github/blob/main/CONTRIBUTING.md) van de organisatie: daar staat per project een formulier, ook zonder Git-ervaring.

## Licentie

EUPL-1.2, zie [LICENSE](LICENSE).

## Het idee
Normen en beleid voor de publieke sector staan nu in tekst: BIO 2.0, ISO 27001, de AVG, interne
beleidsstukken. Of de praktijk daar echt aan voldoet, wordt met de hand getoetst, periodiek, in een
spreadsheet. Dat schaalt niet, veroudert snel en is niet reproduceerbaar.

Policy-as-code draait dat om: je legt een norm of beleidsregel vast als **uitvoerbare, toetsbare regel**,
en laat een machine controleren of de werkelijkheid eraan voldoet. Niet "hebben we een wachtwoordbeleid?"
maar een regel die de daadwerkelijke configuratie leest en zegt: hier wel, daar niet, met bewijs.

Kern, in lijn met de andere Commons-tools:

- **Regelgebaseerd en navolgbaar.** Een norm wordt een expliciete regel die iedereen kan lezen en
  bekritiseren, geen black box.
- **Bewijs, geen aanname.** De regel toetst tegen echte gegevens (configuratie-export, inventaris,
  scanresultaat), niet tegen een vinkje.
- **Herbruikbaar.** Een regel die één publieke organisatie schrijft voor een BIO-maatregel, kan een
  andere direct overnemen. Publiek geld, publieke regels.

## Waar het aan raakt
Dit staat niet los van wat er al is. `iamscan`, `blast-radius` en `security-posture-tool` produceren
juist het soort feitelijke gegevens waar een policy-regel tegen kan toetsen; `grc-platform` en
`procescheck` beheren de normen en processen. Policy-as-code is de laag ertussen: de norm als code die
de feiten toetst.

## Denkrichtingen (nog open)
- Welke regeltaal? Een bestaande standaard (bijvoorbeeld OPA/Rego) of iets eenvoudigers en leesbaarders
  voor niet-ontwikkelaars?
- Beginnen bij één concrete normfamilie (bijvoorbeeld een handvol BIO 2.0-maatregelen) in plaats van het
  hele kader.
- Hoe koppel je een regel aan het bewijs dat de bestaande scan-tools al opleveren?

## Meedenken
Ideeën, een use-case of ervaring met policy-as-code in de publieke sector? Open een
[discussion](https://github.com/security-commons-nl/.github/discussions) of een issue.

Open source onder EUPL v1.2.
