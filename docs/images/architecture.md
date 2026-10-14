# MOOCentral V2 – System Architecture

The following diagram illustrates the main components of MOOCentral V2 and how they interact.



## Main Components

- **Celery Beat:** Schedules recurring scraping tasks.
- **Redis:** Manages the task queue and acts as the message broker.
- **Celery Worker:** Executes scheduled scraping tasks.
- **MOOC Platform Scraper:** Collects course data using Python, Django, and Selenium.
- **Neo4j and Neomodel:** Store and manage course data in a graph database.
- **Data API:** Provides an API interface for interacting with the service.

The system automates the collection, validation, and updating of course information from multiple MOOC platforms.

![MOOCentral V2 System Architecture](mooc-system-architecture.png)
