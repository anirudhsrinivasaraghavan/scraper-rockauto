# scraper-rockauto

## Documentation for Rockauto Scraper
### Introduction
This documentation provides an overview of how to install and use the Rockauto Scraper, which scrapes car part data from the Rockauto website based on the configurations set in config.py.

### Prerequisites
Ensure you have the following installed on your system:
- pip install scrapy wget

### Configuration
Before running the scraper, you need to configure the config.py file to match your target specifications. Here is an example of the config.py file:


```python
target_make = "TOYOTA"
target_model = "TACOMA"
target_year = "2011"
target_engine = "2.7L L4"
target_group = "Brake & Wheel Hub"
target_partname = "Brake Pad"

HOST = 'localhost'
USER = 'root'
PASSWORD = 'password'
DATABASE = 'rockauto'
```

### Explanation of Configuration Parameters:
- target_make: The make of the vehicle (e.g., TOYOTA).
- target_model: The model of the vehicle (e.g., TACOMA).
- target_year: The year of the vehicle (e.g., 2011).
- target_engine: The engine type of the vehicle (e.g., 2.7L L4).
- target_group: The part group (e.g., Brake & Wheel Hub).
- target_partname: The specific part name (e.g., Brake Pad).
- HOST, USER, PASSWORD, DATABASE: Database connection details for saving the scraped data.

### Running the Scraper
Navigate to the directory containing the scraper files:
```sh
scrapy runspider scraper.py
```






