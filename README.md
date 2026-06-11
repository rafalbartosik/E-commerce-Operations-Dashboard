# Olist E-Commerce Operations Dashboard / Pulpit Operacyjny E-Commerce Olist
### Strategic Operations Overview — Power BI

## English Version

### Project Description
An interactive Power BI report analyzing the Brazilian e-commerce marketplace **Olist** (~100,000 orders, 2016–2018). The dashboard is designed for an operations decision-maker and answers three questions across dedicated pages: how the business sells, how reliably it delivers, and where its customers are. All figures use **2017** — the only year with a complete set of months — so seasonal trends and comparisons stay consistent.

The project covers the full BI pipeline: data cleaning in Power Query, a star-schema data model in import mode, DAX measures and calculated columns, and a multi-page, interactive report focused on data storytelling.

### Dashboard Pages
* **Home** — navigation landing page.
* **Sales Overview** — revenue, order volume, unique customers and average order value; payment mix; monthly seasonality; category performance.
* **Delivery & Satisfaction** — delivery time, late-delivery and cancellation rates, review scores; the impact of delivery delays on reviews; regional fulfillment and delivery-accuracy comparisons.
* **Customers & Geography** — geographic reach, state-level order volume, average order value by region, and a filled map of Brazil.

### Tech Stack
* **Tool:** Power BI Desktop
* **Data Model:** Star schema, import mode
* **Data Transformation:** Power Query (M)
* **Calculations:** DAX (measures and calculated columns)
* **Visualizations:** native Power BI visuals
* **Data Source:** Olist Brazilian E-Commerce Public Dataset (Kaggle, CSV)

---

## Wersja Polska

### Opis Projektu
Interaktywny raport w Power BI analizujący brazylijski marketplace e-commerce **Olist** (~100 000 zamówień, 2016–2018). Pulpit jest pomyślany dla osoby zarządzającej operacjami i odpowiada na trzy pytania na osobnych stronach: jak firma sprzedaje, jak niezawodnie dostarcza i gdzie są jej klienci. Wszystkie liczby dotyczą roku **2017** — jedynego z kompletem miesięcy — aby trendy sezonowe i porównania były spójne.

Projekt obejmuje pełny proces BI: czyszczenie danych w Power Query, model w schemacie gwiazdy w trybie importu, miary i kolumny kalkulowane DAX oraz wielostronicowy, interaktywny raport nastawiony na opowiadanie historii danymi.

### Strony Raportu
* **Home** — strona startowa z nawigacją.
* **Sales Overview** — przychód, liczba zamówień, unikalni klienci i średnia wartość zamówienia; struktura płatności; sezonowość miesięczna; wyniki kategorii.
* **Delivery & Satisfaction** — czas dostawy, udział spóźnień i anulowań, oceny; wpływ opóźnień dostaw na oceny; porównania dostaw i terminowości w regionach.
* **Customers & Geography** — zasięg geograficzny, liczba zamówień wg stanu, średnia wartość zamówienia wg regionu i mapa Brazylii.

### Wykorzystane Technologie
* **Narzędzie:** Power BI Desktop
* **Model danych:** schemat gwiazdy, tryb importu
* **Przetwarzanie danych:** Power Query (M)
* **Obliczenia:** DAX (miary i kolumny kalkulowane)
* **Wizualizacje:** natywne wizualizacje Power BI
* **Źródło danych:** Olist Brazilian E-Commerce Public Dataset (Kaggle, CSV)

---

## How to Open / Jak otworzyć
1. Clone the repository / Sklonuj repozytorium: `git clone https://github.com/rafalbartosik/E-commerce-Operations-Dashboard.git`
2. Open `Projekt_Rafał_Bartosik.pbix` in Power BI Desktop / Otwórz `Projekt_Rafał_Bartosik.pbix` w Power BI Desktop.
3. Data is imported into the model, so the report opens with no extra setup / Dane są zaimportowane do modelu, więc raport otwiera się bez dodatkowej konfiguracji.

**Data source / Źródło danych:** [Olist Brazilian E-Commerce Public Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Author / Autor:** Rafał Bartosik
