To-Do List Manager

This Python script acts as a basic to-do list manager, allowing users to manipulate tasks. It includes functions to add, remove, and mark tasks as completed. The script utilizes `datetime` for managing task completion times.

## Functions

### `add_task(name, priority)`
Adds a task with a specified name and priority.

### `remove_task(name)`
Removes a task by name from the completed tasks list.

### `complete_task(name)`
Marks a task as completed and moves it to the completed tasks list.

### `print_tasks(task_list)`
Prints the tasks in the specified task list.

## Usage

### Prerequisites
- Python 3.x

### How to Use
1. Open `todo_manager.py`.
2. Run the script to manage your tasks.
3. Check the console for task management updates.

## Example

```python
import datetime

# Your provided code below
def custom_time_format():
    return datetime.datetime.now().strftime('%H:%M')

current_task = {
    "Groom Cats": 2,
    "Wash Dishes": 1,
    "Laundry": 1,
    "Clean Bedrooms": 3
}

# Add_task, remove_task, complete_task, print_tasks functions here...

if __name__ == "__main__":
    # Functions calls below to demonstrate script functionality
    print_tasks(current_task)
    print("\n\n")
  
    # Other function calls and task manipulations here...
    add_task("Mop Floors", 3)
    print("\n\n")

    remove_task("Clean Bathroom")
    print("\n\n")

    complete_task("Wash Dishes")
    print("\n\n")

    print_tasks(current_task)
    print("\n\n")

    # Other function calls and task manipulations here...

    # Print final task lists
    print_tasks(current_task)
    print("\n\n")
    print_tasks(completed_task)
    print("\n\n")
