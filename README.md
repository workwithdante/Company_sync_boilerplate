# Company Sync

## Structure

```
company_sync/
├── __main__.py: Entry point for the application.
├── config.py: Configuration management.
├── database.py: Database connection and setup.
├── logging_config.py: Logging configuration.
├── utils.py: Utility functions.
├── handlers/
│   ├── __init__.py
│   ├── crm_handler.py: Handles interactions with CRM systems.
│   ├── csv_handler.py: Handles CSV file processing.
│   ├── so_updater.py: Updates Sales Order information.
├── processors/
│   ├── __init__.py
│   ├── csv_processor.py: Processes data from CSV files.
├── repositories/
│   ├── crm_repository.py: Repository for CRM data access.
├── services/
│   ├── so_service.py: Service for managing Sales Orders.
├── strategies/
│   ├── aetna_strategy.py: Strategy for Aetna data processing.
│   ├── base_strategy.py: Base strategy class.
│   ├── oscar_strategy.py: Strategy for Oscar data processing.
├── WSClient/
│   ├── __init__.py
```

## Key Components

- **Main Application**: `__main__.py` serves as the entry point, orchestrating the synchronization process.
- **Configuration**: `config.py` manages application settings and configurations.
- **Database**: `database.py` handles database connections and setup.
- **Handlers**: The `handlers` directory contains modules for interacting with external systems like CRMs and CSV files.
- **Processors**: The `processors` directory includes modules for processing data, such as CSV files.
- **Repositories**: `crm_repository.py` provides data access methods for CRM data.
- **Services**: `so_service.py` manages sales order data and business logic.
- **Strategies**: The `strategies` directory contains different strategies for handling data from various sources like Aetna and Oscar.
- **WSClient**: `WSClient` directory contains modules for web service client.

## Features

- **Data Synchronization**: Synchronizes data between different systems, including CRMs and CSV files.
- **CRM Integration**: Integrates with CRM systems through `crm_handler.py`.
- **CSV Processing**: Processes data from CSV files using `csv_handler.py` and `csv_processor.py`.
- **Sales Order Management**: Manages sales order data using `so_service.py` and `so_updater.py`.
- **Data Processing Strategies**: Implements different strategies for handling data from various sources like Aetna and Oscar.
- **Configurable**: Uses `config.py` for easy configuration of application settings.
- **Logging**: Configured logging using `logging_config.py`.

## License

MIT
