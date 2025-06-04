#  Homora Console – AirBnB Clone Backend

> A command-line interface for managing models and storage – built as the backend foundation of an AirBnB clone.

This project represents the first stage of building a full-featured AirBnB clone. It includes a custom console application that allows users to create, update, show, and delete data objects, with persistent file storage using JSON serialization.

---

##  Project Structure

| Task | Description |
|------|-------------|
| `console.py` | Main CLI interface to interact with objects |
| `models/base_model.py` | Defines the BaseModel for all objects |
| `models/engine/file_storage.py` | Manages JSON-based persistent storage |
| `models/*.py` | Includes various data models – `User`, `Place`, `City`, `State`, `Amenity`, `Review` |
| `tests/` | Unit test cases for model classes and storage logic |

---

## 💻 How to Use

### 🔧 Run the Console

```bash
$ ./console.py
(hbnb)
```

This prompt gives access to various commands that let you interact with stored objects.

###  Core Commands

| Command | Description |
|---------|-------------|
| `create <class>` | Creates an object |
| `show <class> <id>` | Displays object info |
| `destroy <class> <id>` | Deletes an object |
| `all [class]` | Shows all objects or by class |
| `update <class> <id> <attr> <value>` | Updates an object's attribute |
| `quit` or `EOF` | Exits the console |

---

##  Alternative Syntax

You can also use a dot notation syntax:

```bash
User.all()
User.show("id")
User.update("id", {"name": "Alice", "age": 30})
```

---

##  Examples

```bash
(hbnb) create User
(hbnb) show User 1234-5678
(hbnb) update User 1234-5678 name "John"
(hbnb) all
(hbnb) User.all()
(hbnb) quit
```

---

##  Testing

To run unit tests:

```bash
python3 -m unittest discover tests
```

---

##  Technologies Used

- Python 3
- JSON for file storage
- Custom CLI using `cmd` module
- Object-Oriented Programming (OOP)

---

##  License

This project is licensed under the [MIT License](./LICENSE)

---

##  Author

**Monark Patel**  
[LinkedIn](https://www.linkedin.com/in/monark2808) | [GitHub](https://github.com/Monark2808)

---