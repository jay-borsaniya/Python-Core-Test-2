# Task Automation Tool (Command-Line)

## Topic Coverage: Decorators, Error Handling, Generators, Modules, Debugging, File I/O,
Regex, Testing, Scripting

**Duration:** 3–4 hours

---

## Problem Statement

You are tasked with building a Command-Line “Task Automation Tool” for a startup. The  
tool will manage scheduled tasks (like reminders, file cleaners, and log analyzers). It should  
demonstrate mastery of advanced Python concepts.

---

## Requirements

### 1. Core Functionality (40 marks)

● Maintain tasks in a JSON file (tasks.json) with fields: id (int), name (str),  
command (str), schedule (str: daily/weekly/once), status (bool:  
active/inactive).  

● Provide menu options:  
1. Add Task  
2. View All Tasks  
3. Search Tasks (by name using Regex)  
4. Run Task (simulate execution with print(f"Running {command}"))  
5. Deactivate Task  
6. Exit  

---

### 2. Decorators & Error Handling (15 marks)

● Create a decorator @log_exceptions that logs any function errors into  
error.log.  

● Wrap critical functions with this decorator.  

● Use try-except-finally blocks for file I/O operations.  

---

### 3. Generators (10 marks)

● Implement a generator task_stream() that yields tasks one at a time from the  
JSON file.  

● Use it to display tasks without loading all into memory.  

---

### 4. Modules & Debugging (10 marks)

● Split the project into modules:  
○ task_manager.py (CRUD operations)  
○ utils.py (decorators, regex helpers)  
○ main.py (entry point)  

● Use pdb or breakpoint() in one part to demonstrate debugging.  

---

### 5. File I/O & Regex (10 marks)

● Implement regex-based search to filter tasks by partial command/name.  

● Append logs of executed tasks to task_logs.txt.  

---

### 6. Scripting & Career Angle (5 marks)

● Add a feature: if a user runs with --summary, print:  
○ Total tasks  
○ Active tasks  
○ Inactive tasks  

● Add a docstring or readme section discussing how such a scripting tool could be  
part of a Python developer’s career (automation, DevOps, etc.).  

---

## Example Output

1. Add Task  
2. View All Tasks  
3. Search Tasks  
4. Run Task  
5. Deactivate Task  
6. Exit  

Search keyword (regex): clean.*  
Found: [ { "id": 2, "name": "Clean Logs", "command": "rm logs/*",  
"schedule": "daily" } ]  

Running: rm logs/*  
Task executed successfully.  

Summary:  
Total: 5 | Active: 3 | Inactive: 2  

---

## Skills Tested

✅ Advanced Python: decorators, error handling, modules  
✅ Real-world scripting & automation  
✅ File I/O + regex + logs  
✅ Testing culture (unit tests)  
✅ Debugging practice  
✅ Generators for memory efficiency  
✅ Career relevance  
