# 2025 GeoJSON Polska <img width="32" height="32" alt="image" src="https://github.com/user-attachments/assets/3e616e8a-e1c9-4d1a-8ea8-4af989fece5c" /> 🇵🇱 

Zbiór danych granic administracyjnych Polski w formacie **GeoJSON** przygotowany do użycia m.in. w **OpenStreetMap**, **Leaflet** oraz innych aplikacjach mapowych.

---

## GeoJSON województwa

Granice wszystkich województw w Polsce.  
Każdy obiekt zawiera kod TERYT i nazwę województwa w polu `properties`.

---

## GeoJSON powiaty

Granice wszystkich powiatów w Polsce.  
Każdy obiekt zawiera kod TERYT i nazwę powiatu w polu `properties`.

---

## GeoJSON gminy

Granice wszystkich gmin w Polsce.  
Każdy obiekt zawiera kod TERYT i nazwę gminy w polu `properties`.

---

## Źródło danych

- Dane pobrano z [**Geoportalu**](https://www.geoportal.gov.pl) w sierpniu 2025.
- Wykonano transformację układu współrzędnych z **EPSG:2180** (PUWG 1992) do **EPSG:4326 (WGS84)**.  
- Dane są kompatybilne z **OpenStreetMap** oraz **Leaflet**.

---

## Uproszczenie geometrii

Zastosowano metodę **Visvalingam Weighted Area (5%)**, co pozwala znacząco zmniejszyć rozmiar plików przy zachowaniu wysokiej jakości granic.

---

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

---

## Licencja

Dane można używać w dowolnym celu (public domain).

--------
--------
--------
Długi opis:

--------
--------
--------

# 2025 GeoJSON Polska 🇵🇱 <img width="32" height="32" alt="image" src="https://github.com/user-attachments/assets/3e616e8a-e1c9-4d1a-8ea8-4af989fece5c" />

Repozytorium zawiera czwórpoziomowy podział administracyjny Polski - mapa Polski, mapa województw, mapa powiatów, mapa gmin.

<img src="/polska%20geojson.jpg" alt="Polska geojson" width="475" height="475" />

Kompletny zbiór danych granic administracyjnych [Polski](https://github.com/waszkiewiczja/GeoJSON-Polska-Wojewodztwa-Powiaty-Gminy/blob/main/polska.json)
 w formacie GeoJSON. Dane przygotowane na podstawie zasobów **Geoportalu** (sierpień 2025) i zoptymalizowane do wykorzystania w aplikacjach webowych, mobilnych oraz projektach GIS.  

---


## GeoJSON województwa

<img src="/wojewodztwa%20geojson.jpg" alt="województwa geojson" width="475" height="475" />

Plik z granicami wszystkich [województw w Polsce](https://github.com/waszkiewiczja/GeoJSON-Polska-Wojewodztwa-Powiaty-Gminy/blob/main/wojewodztwa.json) w układzie współrzędnych **WGS84 (EPSG:4326)**.  
Każdy obiekt w GeoJSON posiada:  
- `JPT_KOD_JE` – kod TERYT województwa  
- `JPT_NAZWA_` – nazwa województwa  

👉 Idealny do wizualizacji map województw w **OpenStreetMap, Leaflet, Mapbox** i innych bibliotekach mapowych.  

---

## GeoJSON powiaty

<img src="/powiaty%20geojson.jpg" alt="powiaty geojson" width="475" height="475" />

Granice wszystkich [powiatów w Polsce](https://github.com/waszkiewiczja/GeoJSON-Polska-Wojewodztwa-Powiaty-Gminy/blob/main/powiaty.json).  
Każdy rekord zawiera kod **TERYT powiatu** oraz jego **nazwę**, co pozwala na łatwą integrację z innymi zbiorami danych publicznych.

Każdy obiekt w GeoJSON posiada:  
- `JPT_KOD_JE` – kod TERYT powiatu  
- `JPT_NAZWA_` – nazwa powiatu  

👉 Dane powiatowe przydatne do analiz statystycznych, projektów badawczych oraz interaktywnych map powiatów.  

---

## GeoJSON gminy

<img src="/gminy%20geojson.jpg" alt="gminy geojson" width="475" height="475" />

Najbardziej szczegółowy plik – granice wszystkich [gmin w Polsce](https://github.com/waszkiewiczja/GeoJSON-Polska-Wojewodztwa-Powiaty-Gminy/blob/main/gminy.json).  
W `properties` zapisano:  
- `JPT_KOD_JE` – kod TERYT gminy  
- `JPT_NAZWA_` – nazwa gminy  

👉 Doskonały do tworzenia map lokalnych, aplikacji wizualizujących budżety gmin, wyniki wyborów, dane demograficzne czy projekty smart city.  

---

## Źródło i transformacja danych

- Dane pobrano z **Geoportalu** (sierpień 2025).  
- Transformacja układu współrzędnych: **EPSG:2180 (PUWG 1992) → EPSG:4326 (WGS84)**.  
- Pliki są w pełni kompatybilne z **OpenStreetMap, Leaflet, Mapbox** i dowolnym oprogramowaniem GIS obsługującym GeoJSON.

---

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

---

## Licencja

Dane udostępnione na zasadach public domain – można je swobodnie pobierać, edytować i wykorzystywać w dowolnych projektach (komercyjnych i niekomercyjnych).

---

## Dokumentacja systemu TERYT – przykład Nowy Targ

System [**TERYT**](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/ogolna_charakterystyka_systemow_rejestru/ogolna_charakterystyka_systemow_rejestru.aspx?contrast=default) zawiera identyfikatory i nazwy jednostek **zasadniczego trójstopniowego podziału terytorialnego kraju** i jest zbudowany według hierarchicznej numeracji: **województw, powiatów, gmin**.


### Budowa identyfikatora terytorialnego

Identyfikator terytorialny składa się z **trzech członów**, z których każdy ma określone znaczenie:

### Człon I – województwo

- **2 cyfry**  
- Symbol województwa nadany województwom ułożonym w kolejności alfabetycznej  
- Liczby parzyste w przedziale: **02 – 98**

### Człon II – powiat / miasto na prawach powiatu

- **2 cyfry**  
- Symbol powiatu nadany powiatom danego województwa, w kolejności alfabetycznej  
- Miasta na prawach powiatu:  
  - 01–60 → powiaty  
  - 61–99 → miasta na prawach powiatu

### Człon III – gmina / dzielnica / delegatura

- **3 cyfry**  
- Dwie pierwsze cyfry → kolejne liczby gmin (dzielnic, delegatur) w powiecie, w kolejności alfabetycznej, zaczynając od gmin miejskich, następnie wiejskie i miejsko-wiejskie  
- Trzecia cyfra → symbol rodzaju jednostki:

| Cyfra | Rodzaj jednostki |
|-------|----------------|
| 1     | gmina miejska |
| 2     | gmina wiejska |
| 3     | gmina miejsko-wiejska |
| 4     | miasto w gminie miejsko-wiejskiej |
| 5     | obszar wiejski w gminie miejsko-wiejskiej |
| 8     | dzielnice m. st. Warszawy |
| 9     | delegatury w miastach: Kraków, Łódź, Poznań, Wrocław |

---

### Przykład – Gmina Nowy Targ

Kod TERYT dla gminy wiejskiej Nowy Targ: 1211092


### Rozbicie kodu

| Pozycja | Kod  | Znaczenie |
|----------|------|-----------|
| 1–2      | 12   | Województwo **Małopolskie** |
| 3–4      | 11   | Powiat **Nowotarski** |
| 5–6      | 09   | Kolejna gmina w powiecie (alfabetycznie) |
| 7        | 2    | Typ gminy: **wiejska** |

> ⚠️ Uwaga: w TERYT istnieje również **miasto Nowy Targ** (gmina miejska) z innym kodem. Ostatnia cyfra pozwala rozróżnić typ jednostki.


### Podsumowanie

Dzięki TERYT możemy jednoznacznie zidentyfikować każdą jednostkę administracyjną w Polsce: województwo, powiat, gminę oraz typ jednostki.




























