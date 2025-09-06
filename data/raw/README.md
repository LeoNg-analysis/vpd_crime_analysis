Raw CSV files are stored in data/raw/. These files are not modified. Cleaned versions are stored in data/clean/.
| Column             | Type   | Description                                                            | Example                  | Notes / Allowed Values                                |
| ------------------ | ------ | ---------------------------------------------------------------------- | ------------------------ | ----------------------------------------------------- |
| **TYPE**           | string | Crime/offence category reported for the incident.                      | Theft from Vehicle       | Standardized labels from VPD; title case recommended. |
| **YEAR**           | int    | Calendar year of the incident (local time).                            | 2023                     | Use 4-digit year (e.g., 2020–2024).                   |
| **MONTH**          | int    | Month of year (1–12).                                                  | 7                        | Consider also storing a formatted `YYYY-MM` string.   |
| **DAY**            | int    | Day of month (1–31).                                                   | 14                       | Validate against month/year (no 31 in some months).   |
| **HOUR**           | int    | Hour of day in 24-hour clock.                                          | 21                       | 0–23; may be missing for some incidents.              |
| **MINUTE**         | int    | Minute of the hour.                                                    | 30                       | 0–59; often 0 if only hour is known.                  |
| **HUNDRED\_BLOCK** | string | Street block where incident occurred (de-identified to hundred block). | “800 BLOCK GRANVILLE ST” | Do **not** re-identify; keep as provided.             |
| **NEIGHBOURHOOD**  | string | Vancouver neighbourhood of the incident.                               | Downtown                 | One of \~22 VPD neighbourhoods; normalize title case. |
| **X**              | float  | Projected or longitude-like coordinate (de-identified).                | -123.1207                | Use as given; do not infer exact address.             |
| **Y**              | float  | Projected or latitude-like coordinate (de-identified).                 | 49.2827                  | Pair with X; mapping should note privacy adjustments. |
