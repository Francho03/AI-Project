# Podsumowanie wyników projektu

## 1. Statystyki opisowe:

- Wygenerowano podstawowe statystyki opisowe, w tym modę (dominantę) i wariancję dla każdej zmiennej numerycznej w zbiorze danych.
- Utworzono histogramy dla każdej zmiennej, aby zwizualizować rozkład danych.
- Wykresy rozrzutu zostały wykorzystane do pokazania zależności między wybranymi parami zmiennych, takimi jak opóźnienie wylotu i przylotu, odległość lotu i wiek.
- Obliczono macierz korelacji, aby zbadać liniowe zależności między wszystkimi zmiennymi numerycznymi. Wyniki zostały przedstawione na heatmapie.

## 2. Drzewo decyzyjne:

- Zbudowano model drzewa decyzyjnego w celu przewidywania satysfakcji klientów na podstawie innych zmiennych.
- Dane zostały podzielone na zbiór treningowy i testowy, aby ocenić wydajność modelu.
- Dokładność modelu na zbiorze treningowym i testowym została obliczona.
- Przeprowadzono strojenie hiperparametrów (np. min_samples_split) w celu poprawy wydajności modelu.
- Utworzono macierz pomyłek (confusion matrix), aby zwizualizować wydajność modelu w zakresie przewidywania każdej klasy.
- Zidentyfikowano najważniejsze cechy (zmienne) wpływające na satysfakcję klientów na podstawie ważności cech w modelu.
- Zwizualizowano strukturę drzewa decyzyjnego za pomocą wykresu.
- Zastosowano technikę przycinania drzewa (Minimal cost complexity pruning) w celu uproszczenia modelu i potencjalnej poprawy jego wydajności.

## 3. Algorytm centroidów (K-means clustering):

- Wykorzystano algorytm K-means do grupowania klientów na podstawie ich cech.
- Standaryzowano dane numeryczne przed zastosowaniem algorytmu.
- Wyznaczono optymalną liczbę klastrów za pomocą metody "łokcia" (elbow method) i Silhouette Score.
- Przeprowadzono analizę klastrów, badając średnie wartości cech numerycznych i rozkład cech kategorycznych w każdym klastrze.
- Zwizualizowano klastry za pomocą PCA (Principal Component Analysis) w celu redukcji wymiarowości i przedstawienia ich na wykresie dwuwymiarowym.
- Określono znaczenie cech dla każdego klastra na podstawie centroidów.
- Zapisano dane z przypisanymi klastrami do nowego pliku CSV.

## 4. Wnioski:

Projekt pokazał zastosowanie różnych technik analizy danych i uczenia maszynowego do badania danych o satysfakcji klientów linii lotniczych. Wyniki dostarczyły cennych informacji na temat czynników wpływających na satysfakcję, a także umożliwiły segmentację klientów na podstawie ich cech.

### 4.1. Analiza wyników drzewa decyzyjnego i klastrowania

#### Drzewo decyzyjne:
- **Dokładność**: Model osiągnął wysoką dokładność na zbiorach treningowym i testowym (około 95%).
- **Najważniejsze cechy**: Online boarding, Inflight wifi service, Type of Travel.
- **Interpretowalność**: Łatwo zrozumieć, jak model podejmuje decyzje.
- **Przycinanie**: Uproszczenie struktury drzewa i zapobieganie przeuczeniu.

#### Klastrowanie (K-means):
- **Optymalna liczba klastrów**: 3.
- **Charakterystyka klastrów**: Identyfikacja grup klientów o podobnych cechach.
- **Segmentacja klientów**: Personalizacja usług i ofert marketingowych.
- **Wizualizacja**: Ułatwione zrozumienie struktury danych.

### 4.2. Wnioski z analizy:
- Zidentyfikowano najważniejsze czynniki wpływające na satysfakcję.
- Podzielono klientów na grupy o podobnych cechach.
- Uzyskano informacje do personalizacji usług i poprawy satysfakcji.

## 5. Najważniejsze czynniki wpływające na satysfakcję

### 5.1. Drzewo decyzyjne:
- **Online boarding**: Wygoda i oszczędność czasu.
- **Inflight wifi service**: Dostęp do internetu podczas lotu.
- **Type of Travel**: Różne priorytety w zależności od rodzaju podróży.

### 5.2. Klastrowanie:
- **Dodatkowe czynniki**:
  - **Departure/Arrival Delay in Minutes**: Punktualność.
  - **Flight Distance**: Komfort i udogodnienia podczas długich podróży.
  - **Inflight entertainment**: Rozrywka pokładowa.
  - **Seat comfort**: Wygodne siedzenia.
  - **Food and beverages**: Jakość jedzenia i napojów.

## 6. Podsumowanie najważniejszych czynników:
- **Wygoda i oszczędność czasu**: Online boarding, szybki internet, brak opóźnień.
- **Komfort**: Komfort siedzeń, rozrywka pokładowa, jedzenie i napoje.
- **Indywidualne potrzeby**: Rodzaj podróży (służbowa/osobista), długość lotu.
