# 2025 GeoJSON Polska <img width="32" height="32" alt="image" src="https://github.com/user-attachments/assets/3e616e8a-e1c9-4d1a-8ea8-4af989fece5c" /> 🇵🇱 

Zbiór danych granic administracyjnych Polski w formacie **GeoJSON** przygotowany do użycia m.in. w **OpenStreetMap**, **Leaflet** oraz innych aplikacjach mapowych.


## GeoJSON województwa

Granice wszystkich województw w Polsce.  
Każdy obiekt zawiera kod TERYT i nazwę województwa w polu `properties`.

## GeoJSON powiaty

Granice wszystkich powiatów w Polsce.  
Każdy obiekt zawiera kod TERYT i nazwę powiatu w polu `properties`.

## GeoJSON gminy

Granice wszystkich gmin w Polsce.  
Każdy obiekt zawiera kod TERYT i nazwę gminy w polu `properties`.

## Źródło danych

- Dane pobrano z [**Geoportalu**](https://www.geoportal.gov.pl) w sierpniu 2025.
- Wykonano transformację układu współrzędnych z **EPSG:2180** (PUWG 1992) do **EPSG:4326 (WGS84)**.  
- Dane są kompatybilne z **OpenStreetMap** oraz **Leaflet**.

## Uproszczenie geometrii

Zastosowano metodę **Visvalingam Weighted Area (5%)**, co pozwala znacząco zmniejszyć rozmiar plików przy zachowaniu wysokiej jakości granic.

## Struktura plików

Każdy obiekt w pliku GeoJSON zawiera pole `properties` z podstawowymi informacjami:

```
"properties": {
  "JPT_KOD_JE": "1211092",
  "JPT_NAZWA_": "Nowy Targ"
}
```

JPT_KOD_JE – kod jednostki terytorialnej (zgodny z systemem TERYT)

JPT_NAZWA_ – nazwa jednostki administracyjnej (np. gminy, powiatu, województwa)

## Licencja

Dane można używać w dowolnym celu (public domain).

--------
--------
--------
Długi opis

--------
--------
--------

# 2025 GeoJSON Polska 🇵🇱 <img width="32" height="32" alt="image" src="https://github.com/user-attachments/assets/3e616e8a-e1c9-4d1a-8ea8-4af989fece5c" />

![Polska](polska%20geojson.jpg)

Kompletny zbiór danych granic administracyjnych [Polski](/polska.json) w formacie GeoJSON. Dane przygotowane na podstawie zasobów **Geoportalu** (sierpień 2025) i zoptymalizowane do wykorzystania w aplikacjach webowych, mobilnych oraz projektach GIS.  

Repozytorium zawiera trójpoziomowy podział administracyjny Polski:  

## GeoJSON województwa

Plik z granicami wszystkich **województw w Polsce** w układzie współrzędnych **WGS84 (EPSG:4326)**.  
Każdy obiekt w GeoJSON posiada:  
- `JPT_KOD_JE` – kod TERYT województwa  
- `JPT_NAZWA_` – nazwa województwa  

📂 [Pobierz plik GeoJSON województwa](data/wojewodztwa.geojson)  

👉 Idealny do wizualizacji map województw w **OpenStreetMap, Leaflet, Mapbox** i innych bibliotekach mapowych.  

## GeoJSON powiaty

Granice wszystkich **powiatów w Polsce**.  
Każdy rekord zawiera kod **TERYT powiatu** oraz jego **nazwę**, co pozwala na łatwą integrację z innymi zbiorami danych publicznych.  

📂 [Pobierz plik GeoJSON powiaty](data/powiaty.geojson)  

👉 Dane powiatowe przydatne do analiz statystycznych, projektów badawczych oraz interaktywnych map powiatów.  

## GeoJSON gminy

Najbardziej szczegółowy plik – granice wszystkich **gmin w Polsce**.  
W `properties` zapisano:  
- `JPT_KOD_JE` – kod TERYT gminy  
- `JPT_NAZWA_` – nazwa gminy  

📂 [Pobierz plik GeoJSON gminy](data/gminy.geojson)  

👉 Doskonały do tworzenia map lokalnych, aplikacji wizualizujących budżety gmin, wyniki wyborów, dane demograficzne czy projekty smart city.  

---

## Źródło i transformacja danych

- Dane pobrano z **Geoportalu** (sierpień 2025).  
- Transformacja układu współrzędnych: **EPSG:2180 (PUWG 1992) → EPSG:4326 (WGS84)**.  
- Pliki są w pełni kompatybilne z **OpenStreetMap, Leaflet, Mapbox** i dowolnym oprogramowaniem GIS obsługującym GeoJSON.  

## Uproszczenie geometrii

Dla zmniejszenia wagi plików zastosowano algorytm **Visvalingam Weighted Area (5%)**, który redukuje liczbę punktów przy zachowaniu jakości i dokładności granic administracyjnych.  

---

## Struktura plików GeoJSON

Każdy obiekt zawiera w sekcji `properties` podstawowe informacje:  

```json
"properties": {
  "JPT_KOD_JE": "1211092",
  "JPT_NAZWA_": "Nowy Targ"
}
```
JPT_KOD_JE – kod jednostki terytorialnej (TERYT)

JPT_NAZWA_ – nazwa jednostki (gmina, powiat, województwo)

Licencja
📖 Dane udostępnione na zasadach public domain – można je swobodnie pobierać, edytować i wykorzystywać w dowolnych projektach (komercyjnych i niekomercyjnych).












