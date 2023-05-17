# Problem Statement
**This project aims to reduce economic disparities in the United States by using data analysis to identify groups of people who are at risk of poverty or financial struggles. We will use clustering and classification techniques to group people based on their education, healthcare access, and other factors, and evaluate the effectiveness of our models using accuracy and F1 score. The insights we gain will help non-profits, policymakers, and government agencies develop targeted interventions and policies to promote economic equity and help those who need it most.**

# Data Dictionary
| Variable Name | Description | Units | Type | Notes (Oridinal names) |
| --- | --- | --- | --- | --- |
| `AGE` | age of the person | years | numeric | A_AGE |
| `STATE` | FIPS State code of previous residence | state name | string | MIG_ST |
| `FAM_RELATIONSHIP` | family relationship | text | string | A_FAMREL |
| `OUT_POCKET_NONPREM` | out of pocket expenditures for non-premium medical care | dollars | numeric | PMED_VAL |
| `OUT_POCKET_OC` | out of pocket expenditures for over the counter health related spending | dollars | numeric | POTC_VAL |
| `OCCUPATION` | major occupation recode | text | string | A_MJOCC |
| `EDU_LVL` | item 18h - Educational attainment | text | string | A_HGA |
| `MARITAL` | marital status | text | string | A_MARITL |
| `SEX` | gender | text/binary | string | A_SEX |
| `HOUSEHOLD_SUMMARY` | detailed household summary | text | string | HHDREL |
| `MILITARY` | Did you ever serve on active duty in the U.S. Armed Forces? | text | string | PEAFEVER |
| `CERT_REQ` | Is your certification required for your job? Main Job? Job from which you are on layoff? Job at which you last worked? | text | string | PECERT3 |
| `TROUB_BATHE` | Does...have difficulty dressing or bathing? | text | string | PEDISDRS |
| `TROUB_HEAR` | Is...deaf or does ...have serious difficulty hearing? | text | string | PEDISEAR |
| `TROUB_SEE` | Is...blind or does...have serious difficulty seeing even when wearing glasses? | text | string | PEDISEYE |
| `TROUB_ALONE` | Because of a physical, mental, or emotional condition, does...have difficulty doing errands alone such as visiting a doctor’s office or shopping? | text | string | PEDISOUT |
| `TROUB_WALK` | Does...have serious difficulty Walking or climbing stairs? | text | string | PEDISPHY |
| `TROUB_CONC` | Because of a physical, mental, or emotional condition, does...have serious difficulty concentrating, remembering, or making decisions? | text | string | PEDISREM |   
| `HISPANIC` | Are you Spanish, Hispanic, or Latino? | text/binary | string | PEHSPNON |
| `IMMIGR_YR` | When did you come to the U.S. to stay? | years | string | PEINUSYR |
| `CITIZENSHIP` | citizenship group | text | string | PRCITSHP |
| `DISABLED` | Does this person have any of these disability conditions? | text | string | PRDISFLG |
| `RACE` | race | text | string | PRDTRACE |
| `WORK_INDUSTRY` | major industry code | text | string | A_MJIND |
| `LABOR_STATUS` | major labor force recode | text | string | PEMLR |
| `WRK_STATUS` | full/part-time work status | text | string | PRWKSTAT |
| `WRK_CLASS_LONGEST` | longest job class of worker | text | string | LJCW |
| `LONGEST_IND` | industry of longest job by detailed groups | text | string | WEIND |
| `NO_WRK_RSN` | What was the main reason ... did not work in 20..? | text | string | RSNNOTW |
| `FT_PT` | weeks worked recode | text | string | WEWKRS |
| `WEEKS_WRK` | During 20.. in how many weeks did ... work even for a few hours? | text | string | niu, numeric value for the week |
| `EARN_SOURCE` | source of earnings from longest job | text | string | ERN_SRCE |
| `GROSS_PAY` | How much did ... earn from this employer before deductions in 20..? what was ... net earnings from this business/ farm after expenses during 20..? | dollars | numeric | ERN_VAL |     <------ 'ERN_VSL':'GROSS_PAY'
| `ERN_OTR` | wage and salary money earned from other work | text | string | ERN_OTR |
| `EARN_TOTAL` | total wage and salary earnings (combined amounts in ern-val, if ern-srce=1, and ws-val) | dollars | numeric | WSAL_VAL |
| `WORK_DIS` | Who has a health problem or a disability which prevents work or which limits the kind or amount of work? | text | string | DIS_HP |
| `DIS_INC` | What was the source of disability income? | text | string | DIS_SC1 |
| `OTH_DIS_INC` | What was the source of disability income? | text | string | DIS_SC2 |
| `TOTAL_DIS_INC` | total amount of disability income received, combined amounts in edited sources one and two | dollars | numeric | DSAB_VAL | 
| `FIN_ASSIST` | Did ... receive financial assistance? | text | string | FIN_YN |
| `OTH_INC` | other income sources | text | string | OI_OFF |
| `TIME_ASSIST` | In how many months of 20.. did ... receive public assistance payments? | months | numeric | PAW_MON |
| `CASH_ASSIST` | What type of program did... receive CASH assistance? | text | string | PAW_TYP |
| `WIC` | Who received Women, Infants, and Children? | text | string | WICYN |
| `CHLD_SUP` | What is the annual amount of child support paid? | dollars | numeric | CHSP_VAL | 
| `ADJ_GROSS_INC` | federal adjusted gross income | dollars | numeric | AGI |
| `CS_REQ` |  |  |  |  |    <--------- ?????????
| `TAX_FILE_STAT` | tax filer status | text | string | FILESTAT |
| `HEALTH_INS` | any health insurance coverage last year | text | string | COV |
| `PUB_INS` | public coverage last year | text | string | PUB_CYR |
| `PRIV_INS` | private coverage last year | text | string | PRIV_CYR |
| `POV_STS` | supplemental poverty measure (SPM) poverty status | text/binary | string | SPM_POOR |
| `POV_LVL` | poverty level of persons (subfamily members have primary family recode) | text | string | PERLIS |