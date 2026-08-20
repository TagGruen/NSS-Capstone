Solar Flares & Terrestrial Phenomena — Power BI Project (PBIP)

WHAT IS INCLUDED
- Solar_Flares_Earth_Dashboard.pbip
- Solar_Flares_Earth_Dashboard.Report/   (PBIR report definition)
- Solar_Flares_Earth_Dashboard.SemanticModel/ (TMDL semantic model)
- Reference/Solar_Flares_PowerBI_Ready.xlsx
- Reference/PowerBI_Dashboard_Mockup.png

DASHBOARD CONTENT
- KPI card: strongest |r|, lowest FDR-adjusted p, number of significant headline rows
- Bar chart: representative Pearson r for the four terrestrial phenomena
- Headline findings table
- Precipitation lag chart: precipitation-anomaly r and M-class r
- Earthquake lag chart: all-earthquake r and M6+ r

MAIN FINDINGS
- Earthquakes: no robust significant relationship after FDR correction.
- Volcanic eruptions: essentially no relationship.
- Precipitation: small positive association; strongest M-class result at 7 days
  (r = 0.063654, FDR-adjusted p = 0.001170).
- Temperature: no statistically significant short-term relationship.

OPENING THE PROJECT
1. Keep the .pbip file beside both the .Report and .SemanticModel folders.
2. Open Solar_Flares_Earth_Dashboard.pbip in Power BI Desktop.
3. If prompted, enable the Power BI Project (PBIP/PBIR) preview feature and restart Desktop.
4. The semantic model uses embedded Power Query #table data, so it has no external data-source dependency.
5. Because this hand-authored project does not ship a local cache.abf, if visuals are blank at first,
   choose Home > Refresh to load the embedded tables.
6. Use File > Save As to save a normal .pbix file if desired.

IMPORTANT
This PBIP was generated from the analysis results in the accompanying project workbook. The files were
structurally checked here, but Power BI Desktop itself is not available in this environment, so I could
not perform a final Desktop render/open test. PBIP/PBIR is a Microsoft preview-format workflow and may
be upgraded by newer Power BI Desktop builds when opened.


PATCH v2: Removed unsupported layoutOptimization property from PBIR report.json to conform to report schema 3.3.0.
