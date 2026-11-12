# Zbiorkomapa

Interaktywna wizualizacja tras komunikacji miejskiej oparta na danych GTFS. Wybierasz miasto, linię i kierunek — dostajesz trasę na mapie, listę przystanków, długość trasy oraz zapowiedzi głosowe (nagrania lub TTS).

**Strona:** <https://zbiorkomapa.github.io/>

## Obsługiwane miasta

- Poznań
- Świnoujście
- Gorzów Wielkopolski
- Nowy Tomyśl

## Repozytoria

- [danielmroczek/zbiorkomapa](https://github.com/danielmroczek/zbiorkomapa) — kod źródłowy aplikacji, pipeline danych GTFS i mapowanie nagrań głosowych
- [zbiorkomapa/zbiorkomapa.github.io](https://github.com/zbiorkomapa/zbiorkomapa.github.io) — repozytorium artefaktowe: zawartość jest wypychana automatycznie po każdym buildzie, nie edytuj jej ręcznie

## Jak to działa

Skrypty pobierają archiwa GTFS skonfigurowane w `cities.json`, przetwarzają je do lekkich plików JSON dla przeglądarki (trasy, kierunki, kształty, przystanki) i mapują nazwy przystanków na nagrania głosowe lub syntezę mowy. Frontend to statyczna aplikacja oparta na Leaflecie, bez backendu.