# Introduction-to-Computer-Science-Python-Project

## Assignment Description

This project models the hierarchical structure of a futuristic Martian Robot Society using **tree data structures** in Python. 
In the year 3142, robots have established a strict hierarchy on Mars, with each citizen (robot) having specific roles, relationships, 
and possibly leadership over a district.

### Learning Goals
- Model real-world hierarchical data using trees.
- Implement recursive operations (both mutating and non-mutating).
- Practice writing comprehensive test suites.

### Core Concepts
- **Citizen**: Represents a single robot with attributes such as ID, manufacturer, model year, job, and rating. 
  Citizens can have a superior and multiple subordinates.
- **DistrictLeader**: A subclass of Citizen representing a leader of a district. All direct and indirect subordinates belong to their district.
- **Society**: Represents the entire hierarchy, manages citizens, and performs operations on the whole structure.

### Key Features
- Add/remove citizens to/from the hierarchy.
- Retrieve direct/indirect subordinates.
- Find the closest common superior between two citizens.
- Manage district memberships and rename districts.
- Promote citizens based on ratings and reassign roles.
- Delete citizens while preserving hierarchy integrity.

### Structure
- **society_hierarchy.py** – Core logic (to be implemented/modified).
- **society_ui.py** – Graphical interface for interacting with the hierarchy (read-only).
- **client_code.py** – Intermediate layer connecting UI to backend logic (read-only).
- **citizens.csv** – Sample hierarchy data.
- **a2_starter_tests.py** – Starter unit tests.

### Technical Constraints
- No usage of `list.sort` or `sorted` (use provided `merge` helper instead).
- No new public methods/attributes in given classes.
- Must maintain sorted order of citizens by ID where applicable.
- Follow provided docstrings, type hints, and design recipes.

### Usage
Run the UI:
```bash
python society_ui.py
```

Run tests:
```bash
pytest a2_starter_tests.py
```

### Author
This project was developed as part of the University of Toronto CSC148 course requirements.
