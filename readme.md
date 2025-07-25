# UK Rape Crisis Data Analysis: Methodology and Sources

## Overview

This repository contains comprehensive data analysis of rape offences in the United Kingdom from 2002-2029, including projections and true scale estimates accounting for underreporting. The analysis reveals the hidden scale of sexual violence and systemic failures in the justice system.

## Key Findings Summary

- **5+ million people raped** in the UK since 2002 (true scale estimate)
- **Only 2.1% of reported cases** result in criminal charges
- **5 out of 6 rapes** are never reported to police
- **England & Wales has the highest rape rate in Europe** (117.7 per 100,000 vs EU mean of 21.5)
- **99.6% of actual rapists** are never charged with an offence

## Methodology

### Base Data Sources

#### Primary Source: Office for National Statistics (ONS)
- **Source**: Crime in England and Wales: Appendix tables, table A5a
- **Publisher**: Office for National Statistics (UK)
- **Coverage**: England & Wales police recorded crime data
- **Baseline year**: 2002/03 (12,295 recorded rapes)
- **Latest data**: 2023/24 (67,928 recorded rapes)

#### Validation Sources
- **Statista**: UK rape statistics (confirms 71,670 rapes in 2024/25)
- **House of Lords Library**: Rape prosecution statistics
- **European Statistical Data**: Sexual assault rates per 100,000 population

### Geographic Coverage and Adjustments

#### England & Wales Base Data
- Direct from ONS police recorded crime statistics
- Represents approximately 88.8% of UK population
- Forms the foundation for all calculations

#### UK-Wide Projections
- **Scotland adjustment**: Based on population proportion and crime patterns
  - Scotland 2002/03: 924 rapes vs England & Wales 12,295
  - Scotland 2022/23: 2,459 rapes vs England & Wales ~67,000
  - Scotland shows similar trends but lower per-capita rates
- **Northern Ireland adjustment**: Pro-rated based on population
- **Combined UK multiplier**: 1.122 (12.2% increase to account for Scotland & Northern Ireland)

**Important Note**: Analysis shows England & Wales has significantly higher rape rates than European averages. Scotland and Northern Ireland patterns should be validated with official data to ensure accuracy of UK-wide projections.

### True Scale Calculation Methodology

#### Core Formula

```
True Scale = (England & Wales Reported) × (UK Adjustment) × (Underreporting Factor) × (False Allegation Adjustment)
```

#### Detailed Calculation Steps

1. **England & Wales Reported Rapes**
   - Source: ONS police recorded crime data
   - Annual figures from 2002-2023 (actual)
   - 2024-2029 projections using 3.5% annual growth rate

2. **UK Total Adjustment** 
   - England & Wales × 1.122
   - Accounts for Scotland and Northern Ireland
   - Based on population proportions and crime patterns

3. **Underreporting Multiplier: ×6**
   - **Source**: Rape Crisis England & Wales
   - **Methodology**: "Only 1 in 6 rapes are reported to police"
   - **Rationale**: Extensive victim surveys consistently show massive underreporting
   - **Academic support**: Multiple studies confirm 83-85% of rapes go unreported

4. **False Allegation Adjustment: ×0.95**
   - **Rate used**: 5% false allegation rate
   - **Source range**: Academic research shows 2-8% range (Lisak et al., 2010)
   - **Conservative approach**: Used mid-range estimate
   - **Application**: Reduces total by 5% to account for false reports

### Projection Methodology (2024-2029)

#### Growth Rate Calculation
- **Historical baseline**: 2002 (12,295) to 2023 (67,928)
- **Overall increase**: 452% over 21 years
- **CAGR consideration**: Initial calculation showed 8.48% annual growth
- **Adjusted rate**: 3.5% annual growth used for projections (more conservative)
- **Rationale**: Accounts for potential policy interventions and reporting saturation

#### Validation Against Official Data
- **2024 Statista figure**: 71,670 recorded rapes
- **Our 2024 projection**: 70,305 recorded rapes
- **Variance**: <2% difference validates projection accuracy

### Gender Breakdown

#### Statistical Basis
- **Source**: ONS Crime Survey for England and Wales (CSEW)
- **Female victims**: 91% of all rape victims
- **Male victims**: 9% of all rape victims
- **Application**: Applied to all true scale calculations
- **Note**: Percentages reflect both adult and child victims

### Justice System Analysis

#### Charging Rate Data
- **Source**: House of Lords Library - "Rape: Levels of prosecutions"
- **Current rate**: 2.1% of reported cases result in charges
- **Context**: "34.4% increase in charges for adult rape in 2023/24 compared to 2022/23, this still represents a small fraction of all recorded offences"
- **Historical context**: Rate has declined significantly over past decade

#### Calculation Methodology

```
Charged Cases = UK Total Reported × 0.021
Not Charged (Reported) = UK Total Reported - Charged Cases
Not Charged (True Scale) = True Scale Total - Charged Cases
```

### European Context

#### Comparative Data Source
- **Source**: European statistical data on sexual assault rates
- **Metric**: Offences per 100,000 population
- **England & Wales rate**: 117.7 per 100,000 (2021)
- **European mean**: 21.5 per 100,000
- **Second highest (Sweden)**: 96.0 per 100,000
- **UK position**: Highest in Europe, 23% higher than Sweden

## Data Structure

### Primary Data Table Columns

1. **Year**: 2002-2029 (2002-2023 actual, 2024-2029 projected)
2. **E&W**: England & Wales reported rapes (ONS data)
3. **UK Tot**: UK-wide total (E&W × 1.122)
4. **After False Reporting**: True scale after false allegation adjustment
5. **True Scale Female**: Female victims (91% of true scale)
6. **True Scale Male**: Male victims (9% of true scale)
7. **Cumulative Reported**: Running total of reported cases since 2002
8. **Cumulative True Scale**: Running total of true scale cases since 2002
9. **Charged (Reported)**: Cases resulting in charges (2.1% of reported)
10. **NOT Charged (Reported)**: Reported cases with no charges
11. **NOT Charged (True Scale)**: True scale cases with no charges

## Key Assumptions and Limitations

### Assumptions
1. **Consistent underreporting rate**: 1-in-6 rate applied across all years
2. **Uniform false allegation rate**: 5% applied consistently
3. **Linear charging rate**: 2.1% applied to all years (noting actual rate has declined)
4. **Geographic consistency**: UK adjustment factor consistent across time period
5. **Growth rate stability**: 3.5% annual growth sustainable through 2029

### Limitations
1. **Scotland/NI data gaps**: Limited direct data for validation of UK-wide adjustments
2. **Reporting rate changes**: Actual reporting rates may have varied over time
3. **Definition consistency**: Legal definitions and recording practices may have evolved
4. **Charging rate evolution**: Historical charging rates were higher than current 2.1%
5. **Projection uncertainty**: 2024-2029 figures are estimates based on trend analysis

## Data Quality and Validation

### Validation Methods
1. **Cross-reference with Statista**: 2024 projections within 2% of published figures
2. **Growth rate verification**: "Almost sixfold increase" matches our calculated 5.7x
3. **European comparison**: Positions UK appropriately in international context
4. **Academic literature review**: Underreporting and false allegation rates align with research

## Contact and Contributions

This analysis was developed for Rape Crisis UK to support their advocacy and awareness work. 

For questions about methodology or to contribute improvements:
- Review methodology and suggest refinements
- Provide additional validation data sources
- Highlight any calculation errors or assumptions that need revision

## Acknowledgments

- **Rape Crisis England & Wales**: Underreporting statistics and advocacy leadership
- **Office for National Statistics**: Comprehensive crime data provision
- **House of Lords Library**: Justice system prosecution analysis
- **Academic researchers**: Foundational research on false allegation rates and victimization patterns

---

*Last updated: July 2025*
*Data current through: July 25, 2025*