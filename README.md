# Todo List App

A simple command-line Todo List application written in Python. This app allows users to add, remove, and list todo items. The todo list is saved to a file called `todo_list_data.txt`.

## Features

- Add items to the todo list
- Remove items from the todo list
- List all todo items
- Data persistence (todo items are saved to a file)

## Requirements

- Python 3.x

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/todo-list-app.git
    cd todo-list-app
    ```

2. (Optional) Create and activate a virtual environment:
    ```sh
    python -m venv venv
    source venv/bin/activate   # On Windows: venv\Scripts\activate
    ```

## Usage

1. Run the application:
    ```sh
    python todo_list_app.py
    ```

2. Follow the on-screen prompts to add, remove, or list todo items.

## Example

```sh
Todo List App
1. Add item
2. Remove item
3. List items
4. Quit
Choose an option: 1
Enter a new item: Buy groceries

Todo List App
1. Add item
2. Remove item
3. List items
4. Quit
Choose an option: 3
1. Buy groceries



3. **.gitignore**

```gitignore
# Ignore the virtual environment directory
venv/
# Ignore Python cache files
__pycache__/
*.pyc
# Ignore data file
todo_list_data.txt


MIT License

Copyright (c) [year] [your name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

