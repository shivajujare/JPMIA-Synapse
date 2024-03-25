# jpmia-synapse

# Overview

Market-Insight-Analytics is a dedicated sql databae created to analyse the current job trends in the market and create reports. 

First we will create the external tables in the databse pointin to usage view delta tables. Then we create views by joining necessary tables and use these views to load reporting tables.

Below are the main SQL scripts and thier usage
1. 0_schema - to create schema jpmia_ext and jpmia for external and managerd tables respectively
2. 1_ext_tables_uv - DDL scripts to create external tables pointing to uv delta tables
3. 2_jpmia_reporting_DDL - DDL scripts to create managed tables in the databse
4. 3_Load_Ded_pool_tables - Create Stored procedure which loads the data into reporting tables
5. vw_company_detial, vw_job_application_rate, vw_job_detail and vw_top_companies_with_more_jobs - views created by joining multiple tables to create respective reporting tables
6. Analysis - To perform analysis on reporting tables

Questions to answer:
1. State wise Job Report - generate a report at location level by aggregating the jobs at experience level
2. Jobs which have high applicants
3. Domains in order of more job postings
4. Companies reports with theri employees and followers count
5. Find the application rate of each work type at different application type and posting domain level

