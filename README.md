# Docker YAML Experiment

## Overview
This project demonstrates how to use YAML files in a Python application, including reading, displaying, and filtering data. The project is containerized using Docker to ensure consistency across different environments.

## Features
- Read student data from a YAML file
- Display student information
- Filter students based on GPA
- Run the application inside a Docker container

## Prerequisites
Make sure you have the following installed:
- [Python 3.x](https://www.python.org/downloads/)
- [Docker](https://www.docker.com/get-started)
- [Git](https://git-scm.com/downloads)
- [PyYAML Library](https://pyyaml.org/) (installed in the container)

## Project Structure
```
Yaml_Docker/
│-- app.py               # Python application
│-- students.yaml        # YAML file containing student data
│-- Dockerfile           # Docker configuration file
│-- README.md            # Project documentation
```

## Installation & Setup
### 1. Clone the Repository
```sh
git clone https://github.com/cl0ud08/Docker_yaml.git
cd Docker_yaml
```

### 2. Build the Docker Image
```sh
docker build -t yaml-python-app .
```

### 3. Run the Container
```sh
docker run -it yaml-python-app
```

## Usage
1. The application will display all students from the `students.yaml` file.
2. You will be prompted to enter a minimum GPA to filter students.
3. The application will display students who meet the GPA criteria.

## Sample YAML Data (`students.yaml`)
```yaml
students:
  - name: Alice
    age: 21
    major: Computer Science
    gpa: 3.8
  - name: Bob
    age: 22
    major: Mathematics
    gpa: 3.5
```

## Running Without Docker
If you prefer to run the application without Docker:
```sh
pip install pyyaml
python app.py
```

## Contributing
Feel free to contribute by submitting issues or pull requests.

## License
This project is open-source under the [MIT License](LICENSE).

