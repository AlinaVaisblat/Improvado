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
