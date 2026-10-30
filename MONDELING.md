# Mondeling

Het mondeling duurt **20 minuten**.

1. Je laat je website zien.
2. Je krijgt **3 vragen** uit de lijst hieronder.

Je weet van tevoren niet welke 3 vragen je krijgt. Bereid dus **alle** vragen voor.

> 💡 Geef elk antwoord met **je eigen code** erbij. Open het bestand en wijs de regels aan. Een antwoord zonder je eigen code is niet goed.

## Hoe krijg je punten?

Je cijfer bestaat uit twee delen:

| Deel | Wat | Max |
|------|-----|-----|
| 1 | Werken al je userstories? | 4,0 |
| 2 | Je antwoorden op de 3 vragen | 6,0 |

Voor elke vraag krijg je **0, 4 of 8 punten**:

| Punten | Wanneer? |
|--------|----------|
| **0** | Je vindt de code niet. Of je kunt het niet uitleggen. Of je uitleg klopt niet. |
| **4** | Je vindt de code. Je legt uit **wat** de code doet. Soms helpt je docent je een beetje. |
| **8** | Je legt uit **wat** de code doet én **waarom**. Je hebt geen hulp nodig. Je kunt ook een extra vraag beantwoorden, zoals: *"Wat gebeurt er als je deze regel weghaalt?"* |

Je kunt samen maximaal **24 punten** halen. Elke 4 punten is 1 punt van je cijfer:

| Punten | 0 | 4 | 8 | 12 | 16 | 20 | 24 |
|--------|---|---|---|----|----|----|----|
| Deel 2 | 0,0 | 1,0 | 2,0 | 3,0 | 4,0 | 5,0 | 6,0 |

## De vragen

Er zijn vijf groepen vragen (A t/m E). Je krijgt 3 vragen uit **3 verschillende groepen**. Eén vraag komt altijd uit **B. SQL**.

### A. Database

1. Laat je ERD zien. Kies één relatie. Waarom is het een één-op-veel relatie? En waarom staat de foreign key aan die kant?
2. Welke kolom mag leeg blijven (`NULL`)? Waarom mag die leeg zijn? Laat zien waar je dat ziet in je formulier en je code.
3. De rollen staan in een eigen tabel `roles`. Waarom zet je de rol niet als tekst in `users`? Wat gaat er dan mis?
4. Kies een zin uit het verhaal van je opdrachtgever. Welke tabel of kolom heb je daarvan gemaakt? Hoe kwam je daarop?
5. Welk datatype gebruik je voor geld? Waarom niet `FLOAT`?

### B. SQL

6. Laat de query van je filter zien. Hoe ziet de query eruit met één filter? En met twee filters? Hoe maak je dat in PHP?
7. Je keuzelijst gebruikt `DISTINCT`. Wat zie je als je `DISTINCT` weghaalt? Waarom?
8. Laat een `LEFT JOIN` zien die ook rijen **zonder** koppeling laat zien. Welke rijen krijgen `NULL`? Wat verandert er als je er een gewone `JOIN` van maakt?
9. Laat een query zien met `GROUP BY` en `HAVING`. Waarom gebruik je `HAVING` en niet `WHERE`?
10. Kies een getal op je statistiekenpagina. Welke kolomfunctie (`COUNT`, `SUM`, `AVG`, `MIN`, `MAX`) rekent het uit? Hoe komt het getal op de pagina?
11. De bezoeker kiest hoe hij sorteert. Hoe komt die keuze in je `ORDER BY`? Je kunt een kolomnaam niet invullen met een `?`. Hoe heb je dat opgelost?
12. Laat de `INSERT` zien die een nieuwe gebruiker opslaat. Welke kolommen vul je? Waar komt `role_id` vandaan?

### C. Beveiliging

13. Laat een prepared statement zien. Wat is SQL-injectie? Hoe stopt jouw code dat? Wat kan er gebeuren als je de variabele direct in de SQL zet?
14. Waar gebruik je `htmlspecialchars()`? Iemand typt `<script>` in een formulier. Wat gebeurt er als je `htmlspecialchars()` vergeet?
15. Hoe sla je een wachtwoord op? Hoe controleer je het bij inloggen? Waarom vergelijk je het wachtwoord niet met `==`?
16. Laat de rolcheck zien op je logboek of statistiekenpagina. Een medewerker typt die URL in. Wat gebeurt er, stap voor stap?
17. Iemand maakt een account aan. Hoe zorg je dat die geen admin kan worden? Ook niet als hij het formulier verandert in de developer tools?
18. Laat zien hoe je een id uit de URL controleert. Wat gebeurt er bij `?id=abc`? En bij een id dat niet bestaat?
19. Hoe zorg je dat een klant alleen **zijn eigen** reserveringen, boekingen, aanvragen of afspraken ziet?

### D. Wat gebeurt er waar?

20. Kies één formulier. Volg het van begin tot eind: formulier → verwerken → database → doorsturen. Welke bestanden doen mee? Wat gebeurt er in elk bestand?
21. Laat je AJAX zien. Wat stuurt `fetch()` naar de server? Wat stuurt de server terug? Hoe komt dat op de pagina zonder dat die opnieuw laadt?
22. Wat zet je in de sessie als iemand inlogt? Waarom? Wat gebeurt er met de sessie bij uitloggen?
23. Laat je soft delete zien. Wat verandert er in de database als je iets verwijdert? En als je het terugzet? Hoe zorg je dat een bezoeker het verwijderde item niet meer ziet?
24. Hoe komt er een regel in je logboek? Laat zien waar je opslaat wie wat wanneer heeft gedaan.
25. De database werkt niet. Wat ziet de gebruiker dan? Laat je `try`/`catch` zien en hoe de gebruiker op je 500-pagina komt.
26. Een gebruiker laat een veld leeg of vult iets fouts in. Waar controleer je dat? Hoe ziet de gebruiker de foutmelding?

### E. Je code en je keuzes

27. Je docent wijst een regel in je code aan. Wat doet die regel? Waarom staat hij er?
28. Hoe voorkom je dat je dezelfde code vaker schrijft, bijvoorbeeld met `include` of een functie? Staat er nog dubbele code in je project? Hoe zou je die weghalen?
29. Wat zou je de volgende keer anders doen in je project? Waarom?
