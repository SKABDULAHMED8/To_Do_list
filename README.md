class TodoListApp:
    def __init__(self):
        self.data_file = "todo_list_data.txt"
        self.load_data()

    def load_data(self):
        try:
            with open(self.data_file, "r") as f:
                self.todo_list = [line.strip() for line in f.readlines()]
        except FileNotFoundError:
            self.todo_list = []

    def save_data(self):
        with open(self.data_file, "w") as f:
            for item in self.todo_list:
                f.write(item + "\n")

    def add_item(self, item):
        self.todo_list.append(item)
        self.save_data()

    def remove_item(self, item_number):
        try:
            del self.todo_list[item_number - 1]
            self.save_data()
        except IndexError:
            print("Invalid item number")

    def list_items(self):
        for i, item in enumerate(self.todo_list, start=1):
            print(f"{i}. {item}")

    def run(self):
        while True:
            print("\nTodo List App")
            print("1. Add item")
            print("2. Remove item")
            print("3. List items")
            print("4. Quit")
            choice = input("Choose an option: ")

            if choice == "1":
                item = input("Enter a new item: ")
                self.add_item(item)
            elif choice == "2":
                item_number = int(input("Enter the item number to remove: "))
                self.remove_item(item_number)
            elif choice == "3":
                self.list_items()
            elif choice == "4":
                break
            else:
                print("Invalid option")

if __name__ == "__main__":
    app = TodoListApp()
    app.run()
