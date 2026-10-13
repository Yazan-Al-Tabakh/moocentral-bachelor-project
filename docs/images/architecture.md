# MOOCentral V2 – System Architecture

This diagram illustrates the main components of MOOCentral V2 and how they interact.

- **Celery Beat:** schedules recurring scraping tasks.
- **Redis:** manages the task queue.
- **Celery Worker:** executes scraping tasks.
- **MOOC Platform Scraper:** collects course data using Python, Django, and Selenium.
- **Neo4j and Neomodel:** store and manage course data.
- **Data API:** provides the API interface shown in the original architecture.

The system automates the collection and updating of course information from multiple MOOC platforms.
