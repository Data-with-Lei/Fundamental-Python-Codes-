# Fundamental-Python-Codes-

import datetime 
def custom_time_format():
    return datetime.datetime.now().strftime('%H:%M')

current_task = {"Groom Cats": 2, "Wash Dishes": 1, "Laundry": 1, "Clean Bedrooms": 3}

def add_task(name, priority):
    if priority > 3:
        print("Priority must be less than or equal to 3")
        return
    
    current_task[name] = priority
    print(f"Task '{name}'added with priority {priority} ")


completed_task = {"Remove Trash": datetime.datetime.now(), "Cook Dinner": datetime.datetime.now(), "Pickup Medication": datetime.datetime.now(), "Clean Bathroom": datetime.datetime.now()}

# Delete clean bathroom form list2

def remove_task(name):
    if name in completed_task:
        del completed_task[name]    
        print(f"Task '{name}' removed")
    else:
        print("Task not found")

def complete_task(name):
    if name in current_task:
        completed_time = datetime.datetime.now()
        completed_task[name] = completed_time
        del current_task[name]
        formatted_time = completed_time.strftime('%H:%M')
        print(f"Task '{name}' completed at {formatted_time}")
    else: 
        print("Task not found")


def print_tasks(task_list):
    if not task_list:
        print("No tasks found.")
    else:
        print("Tasks:")
        for task, priority in task_list.items():
            print(f"{task} - Priority: {priority}")

if __name__ == "__main__":

 print_tasks(current_task)
print("\n\n")
  
print_tasks(completed_task)
print("\n\n")

add_task("Mop Floors", 3)
print("\n\n")

remove_task("Clean Bathroom")
print("\n\n")

complete_task("Wash Dishes")
print("\n\n")

print_tasks(current_task)
print("\n\n")

print_tasks(completed_task)
print("\n\n")
