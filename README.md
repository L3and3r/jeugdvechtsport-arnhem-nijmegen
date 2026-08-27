# Jeugdvechtsport Arnhem & Nijmegen

Een doorzoekbare, statische webpagina met een zo compleet mogelijk overzicht van
clubs, verenigingen en scholen die **jeugdtraining in vechtsporten** (in de
breedste zin) verzorgen in en rond **Arnhem** en **Nijmegen**.

**Live:** https://l3and3r.github.io/jeugdvechtsport-arnhem-nijmegen/

## Wat zit erin

- ~90 aanbieders, gegroepeerd op hoofddiscipline
- Disciplines: judo, karate, taekwondo, boksen, kickboksen / Muay Thai,
  BJJ / grappling / MMA, jiu-jitsu / zelfverdediging, aikido,
  kung fu / wushu / silat / wing chun, krav maga, capoeira, worstelen, kendo / iaido
- Filteren op stad (Arnhem / Nijmegen / regio), op discipline, op trainingsdag
  voor 14-jarigen, en vrij zoeken
- Per kaart de regel **"Traint 14 jr"**: dag + tijd van de les waar een
  14-jarige in valt (bekend voor ~79 van de 87 clubs; anders "informeer bij club")
- Bovenaan een **"Snelkeuze voor 14-jarigen"**: clubs in Arnhem die op
  ma/di/wo trainen en clubs in Nijmegen die op vrijdag trainen
- Elke kaart linkt door naar de website van de club
- Licht/donker thema

## Bronnen & disclaimer

Samengesteld op basis van openbare bronnen (clubwebsites, gemeentelijke
sportportalen, overzichtssites), laatst gecontroleerd op **27 augustus 2026**.
Lestijden, minimumleeftijden, locaties en tarieven wijzigen regelmatig —
controleer de actuele informatie altijd bij de club zelf.

Correcties en aanvullingen zijn welkom via een issue of pull request.

## Technisch

Eén bestand: `index.html`. Geen build, geen dependencies. De data staat als
JavaScript-array (`CLUBS`) bovenaan het `<script>`-blok; een aanbieder toevoegen
of aanpassen doe je daar. Het optionele veld `t:` bevat de trainingsdag(en) en
-tijd(en) voor 14-jarigen; het dagfilter leest de weekdag-afkortingen
(`ma di wo do vr za zo`) rechtstreeks uit die tekst.
