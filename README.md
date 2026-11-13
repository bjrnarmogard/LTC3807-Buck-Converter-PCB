# LTC3807 Synkron Buck-konverter (5V til 1V, 3A) – Simulering og PCB Design

Dette repositoriet inneholder komplett kretssimulering i **LTspice**, koblingsskjema, 2-lags kretskortutlegg (PCB) i **KiCad**, samt fullstendige produksjonsfiler og dokumentasjon for en synkron step-down (buck) strømforsyning basert på kontrolleren **LTC3807EFE**.

## Tekniske spesifikasjoner
* **Kontroller-IC:** Analog Devices LTC3807EFE
* **Inngangsspenning:** 5V DC
* **Utgangsspenning / Strøm:** 1V DC / 3A
* **Kretskort:** 2-lags PCB (`F.Cu` og `B.Cu`) med sammenhengende jordplan (`GND`) på undersiden for god EMC-skjerming og lav induktans
* **Status:** Verifisert med 0 feil og 0 advarsler i KiCad Design Rule Check (DRC)

## Mappestruktur og innhold
* **`LTspice/`** – Simuleringsfiler (`Buck_converter_5V_til_1V_3A.asc` og `.plt`-oppsett) brukt til å verifisere spenningsregulering og rippel før kretskortutlegg.
* **`Levering/`** – Ferdige produksjons- og dokumentasjonsfiler:
  * **`1_Kortet_i_3D.pdf`** – 3D-visning av overside og underside på det ferdige kretskortet.
  * **`2_Samledokument.pdf`** – Samlet dokumentasjon med koblingsskjema, 2D-utlegg, DRC-rapport (0 feil og 0 advarsler) og komponentliste.
  * **`Gerber/`** – Produksjonsfiler i Protel-format (`.gtl`, `.gbl`, `.gko`, `.gts`, `.gbs`, `.gto`, `.gbo`).
  * **`NC Drill/`** – Excellon borfil (`.TXT`).
  * **`BOM/`** – Komplett komponentliste i Excel (`.xlsx`) beregnet for produksjon av 4 kort med delenumre fra DigiKey.
* **KiCad-prosjektfiler (`TLC3807_prosjekt.*`)** – Komplette kildefiler for skjema (`.kicad_sch`), kretskort (`.kicad_pcb`) og prosjekt (`.kicad_pro`).

---
*Utviklet og dokumentert av Bjørnar Mogård.*
