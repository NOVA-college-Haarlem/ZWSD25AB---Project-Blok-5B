# Eindproject Blok 5B (Hoofdstuk 1 t/m 7 + SQL)

## 📋 Wat ga je doen?

Je bouwt in 4,5 dag een complete webapplicatie voor een **nieuwe opdrachtgever**. Je laat zien dat je alles uit **Hoofdstuk 1 t/m 7** beheerst én de **SQL-stof** van dit blok kunt toepassen: kolomfuncties, `GROUP BY`/`HAVING`, `DISTINCT`, `ORDER BY` en `LEFT JOIN`.

Het thema is nieuw: geen van de thema's uit 5A komt terug. Je mag je **eigen code** uit Eindproject 5A en de projectlessen als voorbeeld gebruiken (bijv. je `database.php`, je login of je header/footer). Je bouwt voor een ander thema, dus kopiëren zonder aanpassen werkt niet.

## 🃏 Zo werkt dit project: kaarten

Je krijgt de opdracht niet in één keer, maar in **6 kaarten**. Elke kaart verschijnt als **Issue** in je repository (tabblad **Issues** op GitHub).

1. Lees de kaart en werk hem af.
2. Klaar? Typ `/klaar` als reactie op de kaart. Je komt dan in de wachtrij van je docent.
3. Je docent komt langs, bekijkt je werk en tekent af door de kaart te sluiten.
4. De volgende kaart verschijnt automatisch. Nog niet goed? Dan krijg je feedback op de kaart - pas aan en typ opnieuw `/klaar`.

Wacht je op je docent? Kijk alvast vooruit in je thema, of help een klasgenoot.

> 📅 **Maandag** werk je zelfstandig aan kaart 1 - er wordt die dag nog niet afgetekend. Typ wel `/klaar` als je klaar bent: dinsdagochtend tekent je docent af in de volgorde van de wachtrij.

## 🎯 Thema's

Je krijgt één van de zes thema's toegewezen - zie **[Studentverdeling.md](Studentverdeling.md)**. Je docent geeft je een nummer; bij dat nummer staat jouw thema. De technische eisen zijn voor alle thema's **exact gelijk**.

1. [Dierenasiel](projects/Dierenasiel.md) - dierenasiel Pootjes & Co
2. [Fietsverhuur](projects/Fietsverhuur.md) - fietsverhuur Trapkracht
3. [Escape Room](projects/EscapeRoom.md) - escape room Locked Inn
4. [Camping](projects/Camping.md) - camping De Duinpan
5. [Kringloop](projects/Kringloop.md) - kringloopwinkel Tweede Ronde
6. [Autogarage](projects/Autogarage.md) - garage Sleutelwerk

## 🚀 Planning van de week

| Dag | Kaart |
|-----|-------|
| **Maandag** | *Ochtend:* toetsen rekenen en AKT. *Middag:* project opzetten en **kaart 1** (ERD), zelfstandig |
| **Dinsdag** | *Ochtend:* kaart 1 aftekenen. Daarna **kaart 2** (database) en **kaart 3** (bezoeker) |
| **Woensdag** | **Kaart 4** (klant) |
| **Donderdag** | **Kaart 5** (medewerker en admin) |
| **Vrijdag** | **Kaart 6** (afronden) - **aan het einde van de dag moet kaart 6 afgetekend zijn** |
| **Week erna** | Mondeling assessment |

> ⚠️ **Vrijdag is de deadline.** Zonder afgetekende kaart 6 kun je de week erna niet mondeling beoordeeld worden. Je hebt maar een halve maandag - zorg dat kaart 1 maandag af is en je `/klaar` hebt getypt, dan word je dinsdag als eerste afgetekend.

## 🛠️ Project setup

Deze repository is een template met een kant-en-klare Docker-omgeving (PHP 8.5 + Apache, MariaDB, PhpMyAdmin en Mailpit).

1. Klik op GitHub op de groene knop **Use this template** en kies **Create a new repository**.
2. Kies bij **Owner** de organisatie `Nova-College-Haarlem-Students` (**niet** je eigen account), anders ziet je docent je kaarten niet. Noem je repository `blok5b-` met daarachter je GitHub-naam, bijvoorbeeld `blok5b-pietjansen`.
3. Ga in je nieuwe repository naar het tabblad **Actions**. Zie je een groene knop om workflows aan te zetten? Klik erop.
4. Kopieer de URL van je repository (via de groene knop **Code**).
5. Open de map waarin je je projecten bewaart met VS Code.
6. Open de terminal en run `git clone <PASTE URL>`.
7. Open het project in VS Code.
8. Verander in `.env` de naam `MYSQL_DATABASE` van "testdb" naar de naam van je project.
9. Zoek in [Studentverdeling.md](Studentverdeling.md) je thema op bij het nummer dat je van je docent hebt gekregen. Maak in de hoofdmap een bestand `thema.txt` met daarin alleen de naam uit de kolom **thema.txt**, bijvoorbeeld `Camping`.
10. Commit en push. Binnen een minuut staat **kaart 1** bij **Issues**.
11. Run in de terminal `docker compose up -d` en controleer of de adressen hieronder werken.

### Beschikbare applicaties

| Applicatie | Adres |
|------------|-------|
| Je webapp | http://localhost |
| PhpMyAdmin (database) | http://localhost:8000 |
| Mailpit (mail) | http://localhost:8025 |
