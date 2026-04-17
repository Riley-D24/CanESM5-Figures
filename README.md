# CanESM5-Figures

A repository containing test code for generating SSP comparison figures based on input data from CanESM5. Figures represent ECCC and NAS at their 2026 Bow River Basin Council (BRBC) presentation.

## Generating Figures

1.    Create a folder titled "CanESM5" in your parent directory. This is where the code will search for your input `.csv` files
2.    Open Python and run `import brbc-postprocessing as brbc`
3.    Run the function `brbc.generate_plot('<station_id>')`, where `<station_id>` is the 7-digit identifier used by ECCC
4.    Alternatively, run the list comprehension `dummy = [generate_plot(plot) for plot in ['<list_of_ids>']]` to generate multiple
5.    A list of applicable stations is available in the file`station_metadata.csv`

## Credit

- Scripts by Riley Damen (Riley.Damen@ec.gc.ca)
- Original data by Sujata Budhathoki (Sujata.Budhathoki@ec.gc.ca)
