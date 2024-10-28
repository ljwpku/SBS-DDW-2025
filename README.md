# SBS-DDW-2025
Snowflake SQL codes for SBS ICD-10 codes EDA for DDW 2025 
All sql codes saved under Snowflake project folder: JL DDW 2025 EDA 
All data tables saved under IRWD private database dev schema: DSVC_IRONWOOD_PRIVATE.DEV_DDW2025_JL

Core codes include
1) Oct 2024: pt_continuous_enrollment:            
       - A locked down version of the dbt model pt_closed_continuous_enrollment to fix the data table for September cohort                      
       - created table: "DSVC_IRONWOOD_PRIVATE.DEV_DDW2025_JL.pt_closed_continuous_enrollment_Oct2024" 
2) Oct 2024: medical_events_tall:                           
       - Locked down version of the dbt model medical_events_tall to fix at September                
       - created table: "DSVC_IRONWOOD_PRIVATE.DEV_DDW2025_JL.MEDICAL_EVENTS_TALL_Oct2024"        
3) Oct 2024 SBS-IF algorithm update:            
       - Locked down and plaid version of the Trinity SBS-IF algorithm                  
       - final patient cohort table: "DSVC_IRONWOOD_PRIVATE.DEV_DDW2025_JL.pt_SBS_step5"

Feasibility option 1. 
  - created active algorithm patients: "DSVC_IRONWOOD_PRIVATE.DEV_DDW2025_JL.PT_SBS_step6_active"             
  - satisfied feasibility assessment, output in SharePoint word             

Option 1 cohort creation:          
  - created final row-level data set for analysis: DSVC_IRONWOOD_PRIVATE.DEV_DDW2025_JL.option1_cohort

Subsequent EDA were done either via Tableau or RStudio                 
