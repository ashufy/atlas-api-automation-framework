# ATLAS – API Test Automation Framework

ATLAS is a scalable, modular API test automation framework built in Python, designed to validate RESTful services in enterprise environments. 
It supports end-to-end testing, including API validation, database verification, and CI/CD integration.

## Key Features

- Fast execution with parallel testing (pytest-xdist)
- API validation using requests
- Database validation using psycopg2
- Modular & reusable design
- Rich reporting with Allure
- CI/CD ready (Jenkins / GitHub)
- Environment-based configurations
- Schema validation using JSONSchema

## Tech Stack

- Python  
- pytest  
- requests  
- psycopg2  
- pytest-xdist  
- Allure Reports 

## Project Structure

ATLAS/
│── tests/
│── datamodels/
│── payloads/
│── utils/
│── configs/
│── routes/
│── reports/
│── testdata/
│── logs/
│── conftest.py
│── requirements.txt
│── pytest.ini
│── README.md

## Setup & Installation

git clone https://github.com/your-username/atlas.git  
cd atlas 
pip install -r requirements.txt

## Running Tests

Run all tests:
pytest

Run in parallel:
pytest -n auto -v

Generate Allure report:
pytest --alluredir=reports  
allure serve reports

## Sample Test Case

def test_get_users():
    response = requests.get("https://api.example.com/users")
    assert response.status_code == 200

## CI/CD Integration

Supports Jenkins and GitHub for automated test execution.

## Future Enhancements

- RAG-based API validation  
- AI-driven test generation  
- Performance testing integration 
- Dashboard monitoring (Grafana)  

## Contribution

Contributions are welcome!

## License

MIT License
