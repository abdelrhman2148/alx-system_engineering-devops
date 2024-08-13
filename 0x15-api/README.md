 VAPI Project

This project focuses on practicing working with APIs, specifically utilizing the JSONPlaceholder REST API. The main objectives were to gather data from the API and export it into either CSV or JSON formats.

## Tasks 📃

 Task 0: Gather data from an API
 
0-gather_data_from_an_API.py:
Python script that retrieves and displays the progress of a to-do list for a specified employee ID.

- **Usage:**  
  ```bash
  python3 0-gather_data_from_an_API.py <employee ID>
  ```
- **Output:**  
  Displays the completion status of tasks for the employee in the format:  
  `Employee <employee name> is done with tasks(<# completed tasks>/<total # tasks>):`

### Task 1: Export to CSV

**1-export_to_CSV.py:**  
Python script that exports to-do list information of a specified employee ID to CSV format.

- **Usage:**  
  ```bash
  python3 1-export_to_CSV.py <employee ID>
  ```
- **File name:**  
  `<employee ID>.csv`
- **Format:**  
  `"employee_id","username","task_completed_status","task_title"`

### Task 2: Export to JSON

**2-export_to_JSON.py:**  
Python script that exports to-do list information of a specified employee ID to JSON format.

- **Usage:**  
  ```bash
  python3 2-export_to_JSON.py <employee ID>
  ```
- **File name:**  
  `<employee ID>.json`
- **Format:**  
  ```json
  {
    "<employee ID>": [
      {
        "task": "<task title>",
        "completed": <task completed status>,
        "username": "<username>"
      },
      ...
    ]
  }
  ```

### Task 3: Dictionary of list of dictionaries

**3-dictionary_of_list_of_dictionaries.py:**  
Python script that exports to-do list information for all employees to JSON format.

- **Usage:**  
  ```bash
  python3 3-dictionary_of_list_of_dictionaries.py
  ```
- **File name:**  
  `todo_all_employees.json`
- **Format:**  
  ```json
  {
    "<employee ID>": [
      {
        "username": "<username>",
        "task": "<task title>",
        "completed": <task completed status>
      },
      ...
    ],
    "<employee ID>": [
      {
        "username": "<username>",
        "task": "<task title>",
        "completed": <task completed status>
      },
      ...
    ]
  }
  ```

