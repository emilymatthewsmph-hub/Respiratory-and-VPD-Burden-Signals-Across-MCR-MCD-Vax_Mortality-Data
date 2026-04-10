# Respiratory-and-VPD-Burden-Signals-Across-MCR-MCD-Vax_Mortality-Data

Planned Outcomes/deliverables

•	Track vaccination coverage (flu, COVID 19, RSV, pneumococcal, selected childhood VPDs) using CDC VaxView/FluVaxView/RSVVaxView. 
•	Track infection/morbidity using surveillance data (FluView, RESP NET, NNDSS where feasible). 
•	Track mortality for respiratory and VPD related ICD 10 causes using NCHS public use mortality.
•	Uses Medicare and  Medicaid public data as a lens on high risk and vulnerable populations.
•	Applies signal detection (rolling baselines, percent change, z scores) to identify unusual burden.


Inital Folder Structure
resp_vpd_burden_signals/
│
├── data_raw/
│   ├── vaxview/
│   ├── fluview/
│   ├── mortality_nchs/
│   ├── medicare_puf/
│   └── medicaid_open/
│
├── data_processed/
│   ├── vaccination_rates/
│   ├── infection_rates/
│   ├── hospitalization_rates/
│   └── mortality_rates/
│
├── src/
│   ├── ingest_vaxview.py
│   ├── ingest_fluview.py
│   ├── ingest_mortality.py
│   ├── ingest_medicare.py
│   ├── classify_vpd_icd.py
│   ├── build_indicators.py
│   ├── detect_signals.py
│   └── plot_trends.py
│
├── outputs/
│   ├── indicators_*.csv
│   ├── signals_*.csv
│   └── plots/
│
└── docs/
    ├── README_draft.md
    ├── methods.md
    ├── data_sources.md
    ├── limitations.md
    └── roadmap.md
