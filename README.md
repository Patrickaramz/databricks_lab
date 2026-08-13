# Marathos Analytics - Databricks Lab

Ett dataprojekt i Databricks Lakehouse som analyserar marathon och friidrottsdata genom en Medallion Architecture (Bronze -> Silver -> Gold).

---

## Task 4: Dimensionell Modellering

I Gold-lagret har datan modellerats i ett star schema för snabb och effektiv analys:

![Dimensional Model](star_schema.png)

### Tabeller i modellen:
* Fakttabell:** `fct_results` (Loppresultat och tider)
* Dimensioner:** 
  * `dim_athlete` (Information om löpare, kön och åldersgrupper)
  * `dim_event` (Information om loppen)

---

## Task 6 & 7: Dashboard & Genie AI Agent

En användarvänlig dashboard i Databricks kopplad till en Genie Agent för ad-hoc-frågor.

### Länkar
* [Marathos Analytics Dashboard](https://dbc-c98f442d-1432.cloud.databricks.com/sql/dashboardsv3/01f19743df641d189d3cf8921e9015b1/pages/a72ea29e?o=7474658504505891)
* [Marathos Genie Chatbot](https://dbc-c98f442d-1432.cloud.databricks.com/genie/rooms/01f19742248612b6bde5b967b60bd7e8?o=7474658504505891)

### Innehåll i Dashboarden
* KPI kort: Totalt antal lopp, resultat och idrottare.
* Diagram: Fördelning av idrottare baserat på kön och åldersgrupper.