# Starlight Academy Enrolment Enquiries
### Automated Data Ingestion Pipeline with Databricks

## Project Overview

The Starlight Academy Enrolment Enquiries project is a data engineering proof of concept demonstrating how enrolment enquiry data can be ingested from Google Sheets into Databricks using managed data ingestion.

A demonstration website was developed using Lovable to simulate an online school enrolment enquiry process. The project uses fictional data and is intended for learning, testing, and portfolio demonstration rather than live school enrolment management.

Google Sheets serves as the source of the enrolment enquiry dataset, while Databricks managed ingestion is configured to access the source through a Google Drive connection and ingest the data into a Databricks table.

The primary focus of this project is establishing and documenting the data ingestion workflow, including source connectivity, pipeline configuration, and data availability in Databricks.

## Project Objectives

- Develop a demonstration enrolment enquiry website using Lovable.
- Use fictional enrolment enquiry data for testing and demonstration.
- Store the source dataset in Google Sheets.
- Configure Databricks managed ingestion using a Google Drive connection.
- Ingest source data into a Databricks table.
- Explore automated data ingestion and source-to-target data movement.
- Document the implementation using screenshots and a CSV dataset.

## Technology Stack

| Technology | Purpose |
|---|---|
| Lovable | Development of the demonstration enrolment enquiry website |
| Google Sheets | Source of the fictional enrolment enquiry data |
| Google Drive | Connection used to access the source data |
| Databricks | Managed data ingestion and destination table |
| CSV | Dataset reference and repository artefact |
| GitHub | Project documentation and storage of screenshots and dataset |

## Data Ingestion Architecture

The project follows this workflow:

**Lovable Demonstration Website → Google Sheets → Google Drive Connection → Databricks Managed Ingestion → Databricks Table**

### 1. Demonstration Website

A website was created using Lovable to simulate an online school enrolment enquiry form. It demonstrates how an online interface could be used to capture prospective student and parent or guardian information.

All project records are fictional. The website is not a live school enrolment system.

### 2. Source Data — Google Sheets

Google Sheets serves as the source dataset for the ingestion pipeline. It contains the fictional enrolment enquiry records used to demonstrate the movement of data between the source and Databricks.

### 3. Source Connectivity

Databricks is configured to access the source data through a Google Drive connection.

The connection was named `bigquery` during setup. This is the configured connection name, not a statement that BigQuery is the source system. The actual source connector is Google Drive.

### 4. Managed Data Ingestion

Databricks managed ingestion is used to ingest the source data into the Databricks environment.

The pipeline configuration establishes the source-to-target ingestion workflow, reducing the need for manual data transfers.

### 5. Databricks Destination Table

The ingested data is made available in a Databricks table for querying and downstream use.

The destination table provides a structured representation of the source dataset and can be used to verify that the ingestion process is working as expected.

### 6. Ingestion Verification

The project can be verified by comparing the source data in Google Sheets with the records available in the Databricks destination table.

This includes checking whether the expected columns and records are present and whether newly added source rows appear after the configured ingestion refresh or pipeline update.

The frequency and availability of new records depend on the configured ingestion mechanism and refresh settings.

## Repository Structure

```text
Starlight-Academy-Enrolment-Enquiries/
│
├── README.md
├── Dataset/
│   └── enrolment_enquiries.csv
│
└── Screenshots/
    ├── lovable_website.png
    ├── enrolment_enquiry_form.png
    ├── google_sheets_source.png
    ├── databricks_connection.png
    ├── managed_ingestion_setup.png
    ├── pipeline_configuration.png
    └── databricks_target_table.png
```

*The filenames are examples. Replace them with the actual filenames in your repository.*

## Project Documentation

The repository primarily contains screenshots and the CSV dataset used in the project.

The screenshots document the main stages of the ingestion workflow, including:

- The Lovable demonstration website.
- The Google Sheets source dataset.
- The Databricks Google Drive connection.
- The managed ingestion configuration.
- The pipeline setup.
- The resulting Databricks destination table.

The CSV dataset provides a portable reference for the fictional enrolment enquiry records.

## Skills Demonstrated

- Data engineering fundamentals.
- Source-to-target data ingestion.
- Google Sheets integration.
- Google Drive connectivity.
- Databricks managed ingestion.
- Data pipeline configuration and troubleshooting.
- Source and destination verification.
- Technical documentation and GitHub version control.

## Conclusion

The Starlight Academy Enrolment Enquiries project demonstrates the implementation of a data ingestion pipeline using Databricks managed ingestion.

By using a Lovable demonstration website, fictional Google Sheets data, and a Google Drive connection, the project illustrates how source data can be ingested into Databricks and made available in a destination table.

This project provides practical experience with data source connectivity, managed ingestion, pipeline configuration, and source-to-target data movement in a cloud data engineering environment.