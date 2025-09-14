# AirBnB Clone Project Description

This project is the first step towards building a simple clone of the AirBnB web app. Here, we focus on creating a **command interpreter** (a console) in Python. The console allows us to create, update, delete, and manage objects that represent different parts of the AirBnB system (like users, places, states, etc.). All the data is saved in a JSON file for persistence.

The main goals of this project are to:

* Learn object-oriented programming in Python.
* Handle data serialization and deserialization (converting objects to and from JSON).
* Build a basic storage engine.
* Practice using a command-line interface.

---

## The Command Interpreter

The console works like a mini shell. It lets you interact with the models through simple commands.

### How to Start

1. Clone the repository and move into the folder:

```bash
git clone <https://github.com/tgabin1/alu-AirBnB_clone.git>
cd alu-AirBnB_clone
```

2. Run the console:

```bash
python3 console.py
```

3. You should see the prompt:

```
(hbnb)
```

Now you can start typing commands!

---

### How to Use It

Here are some of the main commands:

* `create <ClassName>` → creates a new object and prints its id.
* `show <ClassName> <id>` → shows the details of an object.
* `destroy <ClassName> <id>` → deletes an object.
* `all [ClassName]` → shows all objects (or all of a class).
* `update <ClassName> <id> <attr_name> "<attr_value>"` → updates an attribute of an object.
* `quit` or `EOF` → exits the console.

---

### Examples

```
(hbnb) create BaseModel
1234-5678-9012

(hbnb) show BaseModel 1234-5678-9012
[BaseModel] (1234-5678-9012) {'id': '1234-5678-9012', 'created_at': '2025-09-11T12:00:00', 'updated_at': '2025-09-11T12:00:00'}

(hbnb) update BaseModel 1234-5678-9012 name "Brenda"
(hbnb) show BaseModel 1234-5678-9012
[BaseModel] (1234-5678-9012) {'id': '1234-5678-9012', 'created_at': '2025-09-11T12:00:00', 'updated_at': '2025-09-11T12:05:00', 'name': 'Titi'}

(hbnb) all BaseModel
["[BaseModel] (1234-5678-9012) {...}"]

(hbnb) quit
```

---
