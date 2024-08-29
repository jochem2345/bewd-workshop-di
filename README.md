# Introductie

Deze workshop is bedoeld om Dependency Injection toe te passen in een Spring Boot applicatie en is onderdeel van de BEWD
course aan de Hogeschool Arnhem/Nijmegen.

Spring faciliteert meerdere annotaties om Dependency Injection toe te passen. In deze oefening gaan we een aantal
daarvan toepassen.

# Workshop

## 1. Deze workshop clonen

Clone deze git repository zodat je er met je eigen favoriete java IDE mee kunt werken.

## 2. Run de code

Je hebt dit project al eerder gezien en kunt na het runnen weer kijken naar de uitvoer via localhost:8081/movies.

## 3. Identificeer de annotaties die horen bij Dependency Injection

Bekijk de code en bekijk hoe de annotaties die behoren bij Dependency Injection zijn toegepast. Het gaat om de volgende
annotaties:

* @Autowired
* @Service
* @Repository

## 4. Filmtitels injecteren met de @Value annotatie

In de klasse `MovieList` worden de titels van de films in code gezet. Met behulp van Depedency Injection is het ook
mogelijk
deze waarden te injecteren. Ze worden daarvoor eerst als properties toegevoegd aan `application.properties`, waarna
Spring
ze runtime kan injecteren.

Voeg de volgende drie properties en waardes toe aan `application.properties`:

* movie1.title=Dune 2
* movie2.title=Twisters
* movie3.title=Love Actually

Gebruik nu
de [documentatie](https://docs.spring.io/spring-framework/reference/core/beans/annotation-config/value-annotations.html)
op de Spring website om uit te zoeken hoe deze waarden geinjecteerd moeten worden, zodat ze niet langer
hard-coded zijn.