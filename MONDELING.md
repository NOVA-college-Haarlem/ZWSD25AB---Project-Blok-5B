# Mondeling assessment

Het mondeling duurt **20 minuten**. Je laat je werkende applicatie zien en je beantwoordt **3 vragen** uit de lijst hieronder. Welke 3 vragen het worden, kiezen je docenten pas tijdens het mondeling. Bereid dus **alle** vragen voor.

Bij elke vraag laat je het antwoord zien **in je eigen code of database**. Een antwoord uit je hoofd zonder je eigen code telt niet als goed.

## Zo word je beoordeeld

| Onderdeel | Max |
|-----------|-----|
| **Functionaliteit**: werken je userstories? | 5,0 |
| **3 vragen**: per vraag 0, 4 of 8 punten, samen maximaal 24 punten | 5,0 |

Per vraag:

| Punten | Wanneer |
|--------|---------|
| **0** | Je vindt de code niet, je kunt het niet uitleggen, of je uitleg klopt niet. |
| **4**, voldoende | Je vindt de code en legt in je eigen woorden uit **wat** die doet. Soms heb je een hint nodig. Het **waarom** blijft vaag. |
| **8**, goed | Je legt zonder hulp uit **wat** de code doet én **waarom**. Je gebruikt de juiste begrippen en je kunt een doorvraag beantwoorden, zoals *"wat gebeurt er als je dit weghaalt?"* |

Je cijfer voor de vragen is `punten ÷ 24 × 5`. Bijvoorbeeld: 4 + 8 + 4 = 16 punten, dat is 16 ÷ 24 × 5 = **3,3**.

## De vragen

De vragen zijn ingedeeld in vijf onderdelen. Je docenten kiezen 3 vragen uit **3 verschillende onderdelen**, en minimaal één daarvan komt uit **B. SQL**.

### A. Database en ontwerp

1. Laat je ERD zien en kies één relatie. Waarom is die relatie één-op-veel, en waarom staat de foreign key aan die kant?
2. Welke kolom in je database mag `NULL` zijn? Waarom mag die leeg zijn, en waar zie je dat terug in je formulier en je code?
3. Waarom staan de rollen in een aparte tabel `roles` en niet als tekst in `users`? Wat gaat er mis als je het wel als tekst opslaat?
4. Laat een zin uit het verhaal van je opdrachtgever zien en de tabel of kolom die je eruit hebt gehaald. Hoe ben je van die zin naar je ontwerp gekomen?
5. Welk datatype heb je voor geld gebruikt? Waarom dat type en niet `FLOAT`?

### B. SQL

6. Laat de query van je filter zien. Hoe ziet de query eruit als de bezoeker één filter kiest, en hoe bij twee filters? Hoe bouw je dat op in PHP?
7. Laat de keuzelijst van je filter zien die met `DISTINCT` gevuld wordt. Wat zie je als je `DISTINCT` weghaalt, en waarom?
8. Laat een `LEFT JOIN` zien die ook rijen **zonder** koppeling toont. Welke rijen krijgen `NULL`-waardes? Wat verandert er als je er een gewone `JOIN` van maakt?
9. Laat een query met `GROUP BY` en `HAVING` zien. Waarom gebruik je hier `HAVING` en geen `WHERE`?
10. Kies een getal van je statistiekenpagina. Welke kolomfunctie rekent het uit, over welke rijen, en hoe komt het getal op de pagina?
11. Hoe komt de sorteerkeuze van de bezoeker in je `ORDER BY` terecht? Waarom kun je een kolomnaam niet met een `?`-placeholder invullen, en hoe heb je dat opgelost?
12. Laat de `INSERT` van het registreren zien. Welke kolommen vul je, en waar komt de waarde voor `role_id` vandaan?

### C. Beveiliging

13. Laat een prepared statement zien. Wat is SQL-injectie, en hoe voorkomt deze code het? Wat kan er gebeuren als je de variabele direct in de SQL-string zet?
14. Waar gebruik je `htmlspecialchars()`? Wat gebeurt er als iemand `<script>` in een formulier typt en jij `htmlspecialchars()` vergeet?
15. Hoe sla je een wachtwoord op, en hoe controleer je het bij het inloggen? Waarom vergelijk je het wachtwoord niet met `==`?
16. Laat de rolcheck op je logboek of statistiekenpagina zien. Wat gebeurt er stap voor stap als een medewerker die URL intypt?
17. Hoe voorkom je dat iemand die zich registreert admin wordt, ook als die het formulier aanpast in de developer tools?
18. Laat zien hoe je een id uit de URL controleert. Wat gebeurt er bij `?id=abc`, en wat bij een id dat niet bestaat?
19. Hoe zorg je dat een klant alleen **zijn eigen** reserveringen, boekingen, aanvragen of afspraken ziet, en niet die van een ander?

### D. Flow: wat gebeurt er waar?

20. Loop één formulier door van begin tot eind: view → process → database → redirect. Welke bestanden doen mee, en wat gebeurt er in elk bestand?
21. Laat je AJAX-actie zien. Wat stuurt `fetch()` naar de server, wat stuurt de server terug, en hoe komt dat op de pagina zonder dat die herlaadt?
22. Wat zet je bij het inloggen in de sessie, en waarom? Wat gebeurt er met de sessie bij het uitloggen?
23. Laat je soft delete zien. Wat verandert er in de database bij verwijderen en bij herstellen? Hoe zorg je dat een verwijderd item niet meer bij bezoekers verschijnt?
24. Hoe komt een regel in je logboek? Laat zien waar in je code je vastlegt wie wat wanneer heeft gedaan.
25. Wat ziet de gebruiker als de database niet bereikbaar is? Laat je `try`/`catch` zien en hoe de gebruiker op je 500-pagina komt.
26. Wat gebeurt er als een gebruiker een veld leeg laat of iets fouts invult? Waar controleer je dat, en hoe ziet de gebruiker de foutmelding?

### E. Code en keuzes

27. Je docent wijst een willekeurige regel in je code aan. Wat doet die regel, en waarom staat die er?
28. Hoe heb je dubbele code voorkomen, bijvoorbeeld met `include` of een functie? Waar staat nog dubbele code, en hoe zou je die weghalen?
29. Welke keuze in je project zou je de volgende keer anders maken, en waarom?
