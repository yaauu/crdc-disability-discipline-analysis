# CRDC Disability Discipline Analysis

A data analysis project examining disciplinary disparities for students with disabilities using U.S. Department of Education Civil Rights Data Collection (CRDC) data.

## Overview

This project quantifies how students with disabilities experience exclusionary discipline at disproportionate rates compared to their non-disabled peers. The analysis covers national, Texas state, and local district levels (Pflugerville ISD, Round Rock ISD, Austin ISD), with particular relevance for educators serving students with autism and other IDEA-eligible disabilities.

**Data Source:** CRDC 2020-21 (U.S. Dept. of Education, released 2023)

## Key Findings

- Students with disabilities (SWD) are **1.99x** more likely to receive an out-of-school suspension
- - SWD are **2.70x** more likely to receive multiple out-of-school suspensions
  - - Black SWD face the highest absolute OOS suspension rate at **3.46%**
    - - Pflugerville ISD suspends SWD at **10.99%** vs 2.22% nationally — a 3.12x disparity ratio
      - - **81%** of all physical restraint incidents nationally involve IDEA students (14% of enrollment)
        - - Discipline disparities held steady or widened between 2017-18 and 2020-21 despite lower absolute counts due to COVID remote schooling
         
          - ## Repository Structure
         
          - ```
            crdc-disability-discipline-analysis/
            ├── data/                    # Raw and processed CRDC data extracts
            ├── docs/
            │   └── case_study.md        # Full case study write-up (summary version)
            ├── visuals/                 # Charts and visualizations
            └── README.md
            ```

            ## Project Artifacts

            | Artifact | Description | Link |
            |----------|-------------|-------|
            | Case Study (Google Doc) | Full narrative case study with methodology, findings, implications, and recommendations | [View Doc](https://docs.google.com/document/d/19QGJCl_cc4XCZDVbbVoY08IeCWtCItVAip_ebk7zC2o/edit) |
            | Data Workbook (Google Sheets) | Underlying data tables, calculations, and disparity ratios | [View Sheets](https://docs.google.com/spreadsheets/d/1kD_ilAgQm_DaHYtKmvuE3Aj4sXag40_N4z95Rj-3rJY/edit) |
            | Interactive Dashboard (Tableau Public) | Visual exploration of discipline disparities by disability status, race, and geography | [View Dashboard](https://public.tableau.com/app/profile/yauncee.dorty/viz/CRDCDisciplineDisparities-StudentswithDisabilities/Sheet3) |
            | CRDC Public Dashboard | Source data | [civilrightsdata.ed.gov](https://civilrightsdata.ed.gov) |

            ## Methodology

            - **Measures:** In-School Suspension, OOS Suspension (1+ and multiple), Expulsion, Referral to Law Enforcement, School Arrest, Physical Restraint, Mechanical Restraint, Seclusion
            - - **Disparity ratio:** SWD rate ÷ Non-SWD rate
              - - **Denominator:** IDEA-only enrollment (Measure 325) for 2020-21; IDEA + Section 504 for 2017-18
                - - **Geographic scope:** National → Texas (State_Id=44) → Pflugerville ISD (Entity_Id=27342), Round Rock ISD (Entity_Id=27370), Austin ISD (Entity_Id=30255)
                 
                  - ## Data Caveats
                 
                  - - 2020-21 was a COVID year; absolute counts dropped sharply, but disparity *ratios* held or widened
                    - - CRDC suppresses cells with very low counts for student privacy (may appear as 0)
                      - - Rates for small districts rest on fewer students and are statistically noisier
                        - - Physical restraint figures use IDEA-only denominators; all other measures use the broader SWD definition
                         
                          - ## Implications for Autistic Learners
                         
                          - CRDC does not disaggregate discipline by specific IDEA category, but autistic students are part of the IDEA-served population disproportionately subject to restraint, seclusion, and suspension. The data suggest schools default to reactive containment rather than proactive behavioral supports — precisely the population that benefits most from Tier 1/2 PBIS frameworks, sensory-friendly classrooms, and trained co-regulation staff.
                         
                          - ## License
                         
                          - Data sourced from the U.S. Department of Education (public domain). Analysis and documentation in this repository are available for educational use.
