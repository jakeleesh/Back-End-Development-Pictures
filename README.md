# IBM Back-end Capstone Photos Microservice

This is the Pictures microservice created in Flask for main Capstone application. It stores URLs of pictures from past events.

## Description

- Developed using Python and Flask following TDD.
- Create CRUD endpoints for picture as a resource.
- Create health endpoint for the microservice.
- Deployed to IBM Code Engine.
- pytest for unit tests.

## Installation

Use the script to install virtual environment.
'''bash
cd /Back-End-Development-Pictures
bash ./bin/setup.sh
'''

## Usage
'''bash
flask run --debugger --reload

curl --request GET --url http://localhost:5000/health
'''
