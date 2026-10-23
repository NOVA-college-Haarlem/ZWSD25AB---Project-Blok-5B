# Kaarten – uitleg voor de docent

Het project wordt in 6 kaarten uitgedeeld als GitHub Issues, door `.github/workflows/kaarten.yml`.

## Eenmalig instellen

1. Maak in de studenten-organisatie een Actions-variabele aan: **Settings → Secrets and variables → Actions → Variables → New organization variable**.
   - Naam: `DOCENTEN`
   - Waarde: de GitHub-gebruikersnamen van de docenten, gescheiden door komma's, bijvoorbeeld `docent1,docent2`
   - Repository access: alle repositories
2. Controleer bij **Settings → Actions → General** van de organisatie dat Actions aan staat.

Alleen wie in `DOCENTEN` staat, kan een kaart aftekenen. Sluit een student zelf een kaart, dan heropent de workflow hem.

## Tijdens het project

**Je wachtrij** - zet deze zoekopdracht als bladwijzer:

```
https://github.com/issues?q=org:Nova-College-Haarlem-Students+is:issue+is:open+label:aftekenen+sort:created-asc
```   

Wie bovenaan staat, wacht het langst.

**Aftekenen** - sluit de kaart met **Close as completed**. De volgende kaart verschijnt meteen.

**Nog niet goed** - laat een reactie achter en haal het label `aftekenen` weg. De student past aan en typt opnieuw `/klaar`. Sluiten met **Close as not planned** levert ook geen nieuwe kaart op.

**Voortgang** - wie op welke kaart zit:

```
https://github.com/issues?q=org:Nova-College-Haarlem-Students+is:issue+is:open+in:title+Kaart
```

## Hoe het werkt

| Gebeurtenis | Wat de workflow doet |
|-------------|----------------------|
| Student pusht (eerste keer) | Opent kaart 0 (oefenkaart) |
| Student typt `/klaar` | Controleert `thema.txt`, zet label `aftekenen` |
| Docent sluit kaart als completed | Opent de volgende kaart |
| Student sluit kaart zelf | Heropent de kaart |

- Kaartteksten: `.github/kaarten/0.md` t/m `6.md`. Kaart 0 is een oefenkaart: aftekenen als `thema.txt` klopt met `Studentverdeling.md` en Docker draait. De eerste regel is de titel.
- Userstories per thema: `.github/kaarten/userstories/`. Ze komen op kaart 3 (bezoeker + developer), 4 (klant) en 5 (medewerker + admin), op basis van `thema.txt`.
- De kaarten staan in de repository van de student. Wie in `.github` gaat zoeken, kan vooruitlezen.
- Kaart 0 komt niet? Laat de student bij **Actions → Kaarten → Run workflow** de workflow handmatig starten.
