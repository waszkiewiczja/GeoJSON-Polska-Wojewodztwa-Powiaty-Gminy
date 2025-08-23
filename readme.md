# GeoJSON Polska

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

- Dane pobrano z **Geoportalu** w sierpniu 2025.  
- Wykonano transformację układu współrzędnych z **EPSG:2180** (PUWG 1992) do **EPSG:4326 (WGS84)**.  
- Dane są kompatybilne z **OpenStreetMap** oraz **Leaflet**.

## Uproszczenie geometrii

Zastosowano metodę **Visvalingam Weighted Area (5%)**, co pozwala znacząco zmniejszyć rozmiar plików przy zachowaniu wysokiej jakości granic.

## Struktura plików

Każdy obiekt w pliku GeoJSON zawiera pole `properties` z podstawowymi informacjami:

```json
"properties": {
  "JPT_KOD_JE": "1211092",
  "JPT_NAZWA_": "Nowy Targ"
}```
JPT_KOD_JE – kod jednostki terytorialnej (zgodny z systemem TERYT)

JPT_NAZWA_ – nazwa jednostki administracyjnej (np. gminy, powiatu, województwa)

## Licencja

Dane można używać w dowolnym celu (public domain).
