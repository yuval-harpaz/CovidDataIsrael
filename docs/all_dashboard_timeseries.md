# Table "[all_dashboard_timeseries.csv](https://github.com/erasta/CovidDataIsrael/blob/master/out/csv/all_dashboard_timeseries.csv)"
## Variable names, their meaning, and sources. 
The table is based on Israel Ministry of Health's [dashboard](https://datadashboard.health.gov.il/COVID-19/general?utm_source=go.gov.il&utm_medium=referral). The data is available as different json files as specified below.  

| field | MOH field | json | description |
| ------ | ------ | - | - |
| date | yyyy-mm-dd |  |  |
| cases | amount | infectedPerDate | positive PCR and Antigen tests by reported date | 
| recovered | recovered | infectedPerDate | recovered cases | 
| tests | amountPersonTested | infectedPerDate | PCR and Antigen tests for COVID diagnosis (not recovery) |
| positiveRate | positiveRate | infectedPerDate | percent positive tests = 100×cases/tests | 
| positiveRatePCR | positiveRatePCR | infectedPerDate | percent positive PCR tests | 
| positiveRateAntigen | positiveRateAntigen | infectedPerDate | percent positive Antigen tests | 
| deaths |  countDeaths | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | deaths by date of death |
| countHardStatus | countHardStatus | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | hospitalized severely ill patients (low oxygenation, PaO2/FiO2 < 300) |
| countMediumStatus | countMediumStatus | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | hospitalized in medium condition (COVID19 + pneumonia) |
| countEasyStatus | countEasyStatus | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | hospirtalized in mild condition (some COVID19 symptoms) |
| severeNew | seriousCriticalNew | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | new hospitalized patients in severe condition |
| mediumNew | mediumNew | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | new hospitalized patients in medium condition (may have improved from severe)|
| easyNew | easyNew | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | new hospitalized patients in mild condition (may have improved from mild or severe)|
| countBreath | countBreath | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | mechanically ventilated patients |
| countCriticalStatus | countCriticalStatus | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | hospitalized in critical condition (system failure- heart, lungs, kidneys...). usually in ICU |
| countEcmo | countEcmo | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | patients connected to ECMO |
| countBreathCum | countBreathCum | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | cumulative mechanically ventilated patients |
| newHospitalized | newHospitalized | [hospitalizationStatus](https://datadashboardapi.health.gov.il/api/queries/hospitalizationStatus) | new hospital admissions |


