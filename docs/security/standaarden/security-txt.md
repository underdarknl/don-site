---
tags:
  - "security"
  - "security-by-design"
title: "Security.txt"
---

De security.txt standaard zorgt ervoor dat ethische hackers laagdrempelig
kwetsbaarheden kunnen melden bij de eigenaar/ beheerder van een applicatie.

## Path

Het bestandje wordt op de volgende plek geplaatst:

`https://voorbeeld.nl/.well-known/security.txt`

Let er op dat de oude locatie 

`https://voorbeeld.nl/security.txt`

Niet meer valide is.

## Genereren met een tool

Voor het genereren van een security.txt heeft
[securitytxt.org](https://securitytxt.org/) een aan te bevelen tool.

## Toepasbaar op websites en API's

De security.txt standaard geldt voor zowel websites als API's. Achter beide type
applicaties zitten levende codebases die kwetsbaarheden kunnen bevatten en die
onderhoud vergen.

## Doorverwijzen naar een centrale security.txt

Sommige organisaties hebben een centrale security.txt waarnaar alle diensten
doorverwijzen middels een 302 redirect. Een organisatie zoals het CBS (Centraal
Bureau voor de Statistiek) doet dit. Je vindt het security.txt bestand van het
CBS [hier](https://www.cbs.nl/.well-known/security.txt).

Het voordeel hiervan is dat er maar één security.txt up-to-date gehouden moet
worden. Een nadeel hiervan kan zijn dat het niet direct helder is welke afdeling
of welk persoon er verantwoordelijk is voor de dienst. Hier moet degene die in
contact wil komen met de beheerder dan achter komen via de het algemene
e-mailadres die in het centrale security.txt bestand staat.

Voor Rijksoverheden is het ook gebruikelijk om naar de security.txt van het NSCS 
te wijzen.

## Waar moet ik op letten?

In de security.txt wordt een einddatum opgenomen, deze mag niet te ver in de 
toekomst liggen (doorgaans accepteren tools 1 jaar), en niet in het verleden, 
maak dus een agenda reminder voor het team dat veranwoordelijk is voor de 
afhandeling van de binnenkomende berichten om deze security.txt periodiek te
herzien.

Idealiter neem je ook een PGP sleutel op in het bericht om er voor te zorgen 
dat communicatie over (ernstige) kwetsbaarheden zeker weten alleen door de 
aangewezen ontvanger gelezen kan worden. Je wilt immers niet dat een 
tussenpartij of wellicht verkeerde mail-forward een aanval kan veroorzaken.

## Meer informatie

Meer informatie over hoe je als organisatie om moet gaan met de security.txt
standaard vind je hier:
[www.digitaltrustcenter.nl](https://www.digitaltrustcenter.nl/securitytxt)
