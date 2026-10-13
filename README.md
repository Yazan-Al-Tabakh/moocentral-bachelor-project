# MOOCentral V2 – Automated MOOC Data Collection and Management

**Bachelor's Thesis Project | University of Duisburg-Essen | 2025**

## Overview

MOOCentral V2 is an enhanced system for collecting, updating, and managing course data from multiple Massive Open Online Course (MOOC) platforms.

This project was developed as part of my Bachelor's thesis, *Improving Data Collection and Management in MOOCentral*. It builds upon an existing system and focuses on improving automation, scraping efficiency, data consistency, and periodic updates.

## Key Features

- **Automated Web Scraping:** Extracting course information from multiple online learning platforms using Python and Selenium.
- **Periodic Updates:** Scheduling recurring scraping tasks to keep course information up to date.
- **Change Detection:** Using hashing techniques to identify modified course content and reduce unnecessary database updates.
- **Data Management:** Storing course information and relationships in a Neo4j graph database.
- **Background Processing:** Using Celery and Redis to schedule and execute scraping tasks.
- **Data Quality:** Identifying new courses, updating existing records, and removing outdated courses.

## Architecture

The system combines the following components:

1. **Django and Python** – Backend functionality and data collection workflows.
2. **Selenium** – Browser automation and extraction of dynamic web content.
3. **Celery Beat and Redis** – Scheduling and queuing periodic scraping tasks.
4. **Celery Workers** – Executing scraping tasks.
5. **Neo4j and Neomodel** – Storing and managing course data in a graph database.

## Evaluation Results

The evaluation in my Bachelor's thesis compared MOOCentral V2 with its predecessor, MOOCentral V1.

- **57.8% average improvement in execution time** across the evaluated MOOC platforms.
- **100% completeness** on most evaluated platforms.
- **100% exactness** for extracted attributes in most cases.
- Udemy completeness reached approximately **32.87%**, reflecting platform scale and execution constraints.

The evaluation focused on execution time, completeness, and exactness.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming language | Python |
| Backend framework | Django |
| Web scraping | Selenium |
| Graph database | Neo4j |
| Object-graph mapping | Neomodel |
| Task scheduling | Celery Beat |
| Background processing | Celery |
| Message broker | Redis |

## Academic Information

- **Thesis:** Improving Data Collection and Management in MOOCentral
- **Degree:** Bachelor's thesis in Computer Science
- **Institution:** University of Duisburg-Essen
- **Year:** 2025

## Repository Note

This repository presents an overview of the project, its architecture, and its evaluation. The original source code is maintained in a university-owned repository and is not included here.

## Author

Mhd Yazan Al Tabakh
