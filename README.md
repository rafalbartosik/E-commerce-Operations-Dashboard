# Olist E-Commerce Operations Dashboard / Pulpit Operacyjny E-Commerce Olist
### Strategic Operations Overview — Power BI

## English Version

### Project Description
An interactive Power BI report analyzing the Brazilian e-commerce marketplace **Olist** (~100,000 orders, 2016–2018). The dashboard is designed for an operations decision-maker and answers three questions across dedicated pages: how the business sells, how reliably it delivers, and where its customers are. All figures use **2017** — the only year with a complete set of months — so seasonal trends and comparisons stay consistent.

The project covers the full BI pipeline: data cleaning in Power Query, a star-schema data model in import mode, DAX measures and calculated columns, and a multi-page, interactive report focused on data storytelling.

### Key Features
* **Star-schema model (import mode):** one fact table, conformed dimensions, a calendar table, a dedicated measures table, and a disconnected helper table for banding.
* **Explicit DAX measures only** — no aggregated columns dragged onto visuals; clear, descriptive names.
* **Dual date relationships** handled with `USERELATIONSHIP` (active order date + inactive delivery date).
* **Disconnected `DeliveryBuckets` table** read via `SELECTEDVALUE` to band orders by delivery delay.
* **Conditional formatting:** traffic-light KPI cards and best/worst bar highlighting.
* **Bookmarks** to toggle two analytical views on a single page (Reviews / Deliveries & Demand).
* **Page navigation, slicers** (Year, Product Category, Review Score) and cross-filtering.
* **Insight-driven chart titles** and a custom map tooltip (revenue, market share, AOV, volume per state).

### Dashboard Pages
* **Home** — navigation landing page.
* **Sales Overview** — revenue, order volume, unique customers and average order value; payment mix; monthly seasonality; category performance.
* **Delivery & Satisfaction** — delivery time, late-delivery and cancellation rates, review scores; the impact of delivery delays on reviews; regional fulfillment and delivery-accuracy comparisons.
* **Customers & Geography** — geographic reach, state-level order volume, average order value by region, and a filled map of Brazil.

### Key Insights
* Sales rise through the year and peak in November (Black Friday); ~4 in 5 orders are paid by credit card.
* Delivery delays sharply lower satisfaction: on-time orders average 4.2★, while orders 8+ days late fall to 1.7★.
* **Slow is not the same as late** — the North has the longest delivery times, but the Northeast misses its promised dates most often.
* São Paulo and the Southeast drive sales volume, while the North has the highest average order value despite the slowest delivery and only ~2% of orders.

### Tech Stack
* **Tool:** Power BI Desktop
* **Data Model:** Star schema, import mode
* **Data Transformation:** Power Query (M)
* **Calculations:** DAX (measures and calculated columns)
* **Visualizations:** native Power BI visuals + Azure Maps
* **Data Source:** Olist Brazilian E-Commerce Public Dataset (Kaggle, CSV)

---

## Wersja Polska

### Opis Projektu
Interaktywny raport w Power BI analizujący brazylijski marketplace e-commerce **Olist** (~100 000 zamówień, 2016–2018). Pulpit jest pomyślany dla osoby zarządzającej operacjami i odpowiada na trzy pytania na osobnych stronach: jak firma sprzedaje, jak niezawodnie dostarcza i gdzie są jej klienci. Wszystkie liczby dotyczą roku **2017** — jedynego z kompletem miesięcy — aby trendy sezonowe i porównania były spójne.

Projekt obejmuje pełny proces BI: czyszczenie danych w Power Query, model w schemacie gwiazdy w trybie importu, miary i kolumny kalkulowane DAX oraz wielostronicowy, interaktywny raport nastawiony na opowiadanie historii danymi.

### Główne Funkcje
* **Model w schemacie gwiazdy (tryb importu):** jedna tabela faktów, wymiary, tabela kalendarzowa, dedykowana tabela miar i odłączona tabela pomocnicza do przedziałów.
* **Wyłącznie jawne miary DAX** — żadnych przeciąganych kolumn z agregacją na wizualizacjach; czytelne, opisowe nazwy.
* **Dwie relacje do daty** obsłużone przez `USERELATIONSHIP` (aktywna data zamówienia + nieaktywna data dostawy).
* **Odłączona tabela `DeliveryBuckets`** odczytywana przez `SELECTEDVALUE` do grupowania zamówień wg opóźnienia dostawy.
* **Formatowanie warunkowe:** karty KPI w stylu sygnalizacji świetlnej i podświetlanie najlepszego/najgorszego słupka.
* **Zakładki (bookmarks)** przełączające dwa widoki analityczne na jednej stronie (Reviews / Deliveries & Demand).
* **Nawigacja między stronami, fragmentatory** (Rok, Kategoria produktu, Ocena) i filtrowanie krzyżowe.
* **Tytuły wykresów niosące wniosek** oraz niestandardowa etykietka mapy (przychód, udział w rynku, AOV, liczba zamówień na stan).

### Strony Raportu
* **Home** — strona startowa z nawigacją.
* **Sales Overview** — przychód, liczba zamówień, unikalni klienci i średnia wartość zamówienia; struktura płatności; sezonowość miesięczna; wyniki kategorii.
* **Delivery & Satisfaction** — czas dostawy, udział spóźnień i anulowań, oceny; wpływ opóźnień dostaw na oceny; porównania dostaw i terminowości w regionach.
* **Customers & Geography** — zasięg geograficzny, liczba zamówień wg stanu, średnia wartość zamówienia wg regionu i mapa Brazylii.

### Kluczowe Wnioski
* Sprzedaż rośnie przez cały rok i szczytuje w listopadzie (efekt Black Friday); ~4 na 5 zamówień opłacanych jest kartą.
* Opóźnienia dostaw mocno obniżają satysfakcję: zamówienia na czas mają średnio 4,2★, a spóźnione o 8+ dni spadają do 1,7★.
* **Wolny to nie to samo co spóźniony** — Północ ma najdłuższe czasy dostawy, ale to Północny Wschód najczęściej nie dotrzymuje obiecanego terminu.
* São Paulo i Południowy Wschód napędzają wolumen sprzedaży, podczas gdy Północ ma najwyższą średnią wartość zamówienia mimo najwolniejszej dostawy i tylko ~2% zamówień.

### Wykorzystane Technologie
* **Narzędzie:** Power BI Desktop
* **Model danych:** schemat gwiazdy, tryb importu
* **Przetwarzanie danych:** Power Query (M)
* **Obliczenia:** DAX (miary i kolumny kalkulowane)
* **Wizualizacje:** natywne wizualizacje Power BI + Azure Maps
* **Źródło danych:** Olist Brazilian E-Commerce Public Dataset (Kaggle, CSV)

---

## How to Open / Jak otworzyć
1. Clone the repository / Sklonuj repozytorium: `git clone https://github.com/rafalbartosik/E-commerce-Operations-Dashboard.git`
2. Open `Projekt_BR.pbix` in Power BI Desktop / Otwórz `Projekt_BR.pbix` w Power BI Desktop.
3. Data is imported into the model, so the report opens with no extra setup / Dane są zaimportowane do modelu, więc raport otwiera się bez dodatkowej konfiguracji.

**Data source / Źródło danych:** [Olist Brazilian E-Commerce Public Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

Project developed as part of university coursework at the Faculty of Mathematics and Computer Science (WMI), Adam Mickiewicz University in Poznań. / Projekt przygotowany w ramach zajęć na Wydziale Matematyki i Informatyki (WMI) Uniwersytetu im. Adama Mickiewicza w Poznaniu.

**Author / Autor:** Rafał Bartosik
