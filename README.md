# Improvado
### Hi and welcome! 👋

Please find below the solution for Senior Marketing Analyst - Technical Assignment

**Setup:**
1. Database Setup: I've used **Big Query Sandbox** for transformations

3. Dashboard: I've used **Tableau Public**

**Deliverables:**

  Link to live **dashboard** (required): https://public.tableau.com/app/profile/alinavaisblat/viz/AV_Imp/ChannelPerformance

  SQL script used for data transformation and unified model creation:

  1. "Improvado_Joining_CSVs" - SQL script unifying 3 csv files provided, keeps all the data. Data is saved to BigQuery table "unified_ads_data".
https://console.cloud.google.com/bigquery?ws=!1m7!1m6!12m5!1m3!1salina-vaisblat-improvado!2sus-central1!3s047b4608-f8cb-47a5-a00e-96e6d5ff6b1e!2e1

  2. "Improvado_Tableau_Ready_Query" - additional SQL script that creates a table, ready to be used in Tableau/other reports aimed at channel comparison (some calculated metrics, no extra columns). Data is saved to BigQuery table "tableau_ready_data". In real life I would use this table in Tableau (via Big Query connector), but I had to build dashboard with the .csv copy of this table due to Tableau Public limitations.
https://console.cloud.google.com/bigquery?ws=!1m7!1m6!12m5!1m3!1salina-vaisblat-improvado!2sus-central1!3scf873711-064c-434a-91b3-e4072f8153e1!2e1

**Notes:**

Below I'll  provide some comments to better explain my work and insights found during the analysis.

_Assumptions:_

  1. Target Audience -	Management (need to see the whole picture to compare channels, without excessive details)
  
  2. "Conversion"	means the same accross all 3 csv files provided

  3. "Spend/Cost" currency is the same across all 3 csv files provided

_Comments about data:_

  1. Jan 31 is missing	If it's extract for a month, I would double check why the last day of the month is missing

  2. No info on conversion value from FB/TT, so can't compare, I would check if it is possible to bring these data to raw tables to enhance analytical opportunities

  3. I've done some data quality checks manually but with the real pipeline it makes sense to include automated tests

_Insights:_

**TLDR:**
Facebook seems to be the best channel in terms of CPA but most of the budget is used for other channels.
In order to optimize CPA even further it makes sense to avoid bidding on high-CPA windows (weekends).

Details:

  1. Jan 31 is missing	If it's extract for a month, I would double check why the last day of the month is missing

  2. No info on conversion value from FB/TT, so can't compare, I would check if it is possible to bring these data to raw tables to enhance analytical opportunities

  3. I've done some data quality checks manually but with the real pipeline it makes sense to include automated tests

