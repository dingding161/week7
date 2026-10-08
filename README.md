# week7
fruits = ["mango", "banana", "orange", "apple"]
print("First fruit:", fruits[0])
print("Last fruit:", fruits[-1])
fruits.append("pineapple")
print("After adding:", fruits)
fruits.remove("banana")
print("After removing:", fruits)
print("Number of fruits:", len(fruits))
fruits = ["mango", "banana", "orange", "apple"]

print("First fruit:", fruits[0])
print("Last fruit:", fruits[-1])

fruits.append("pineapple")
print("After adding:", fruits)

fruits.remove("banana")
print("After removing:", fruits)

print("Number of fruits:", len(fruits))
python list_warmup.py
First fruit: mango
Last fruit: apple
After adding: ['mango', 'banana', 'orange', 'apple', 'pineapple']
After removing: ['mango', 'orange', 'apple', 'pineapple']
Number of fruits: 4
shopping_list = []
while True:
    command = input("Choose: add / remove / show / done: ").lower()

    if command == "add":
        item = input("Enter item: ")
        shopping_list.append(item)
        print("Item added.")

    elif command == "remove":
        item = input("Enter item to remove: ")

        if item in shopping_list:
            shopping_list.remove(item)
            print("Item removed.")
        else:
            print("That item is not on your list.")

    elif command == "show":
        print("Shopping list:")
        for item in shopping_list:
            print(item)

    elif command == "done":
        print("Goodbye!")
        break

    else:
        print("Invalid option.")
        Choose: add / remove / show / done: add
Enter item: bread
Item added.

Choose: add / remove / show / done: add
Enter item: milk
Item added.

Choose: add / remove / show / done: add
Enter item: tea
Item added.

Choose: add / remove / show / done: remove
Enter item to remove: milk
Item removed.

Choose: add / remove / show / done: remove
Enter item to remove: sugar
That item is not on your list.

Choose: add / remove / show / done: show
Shopping list:
bread
tea

Choose: add / remove / show / done: done
Goodbye!
items = ["bread", "avocado", "milk", "sweet potatoes", "tea"]
number = 1

for item in items:
    print(f"{number}. {item}")
    number += 11. bread
2. avocado
3. milk
4. sweet potatoes
5. tea
count = 0

for item in items:
    if len(item) > 4:
        count += 1

print("Items with more than 4 letters:", count)
longest = ""

for item in items:
    if len(item) > len(longest):
        longest = item

print("Longest item:", longest)
items = ["bread", "avocado", "milk", "sweet potatoes", "tea"]

number = 1

for item in items:
    print(f"{number}. {item}")
    number += 1

count = 0

for item in items:
    if len(item) > 4:
        count += 1

print("Items with more than 4 letters:", count)

longest = ""

for item in items:
    if len(item) > len(longest):
        longest = item

print("Longest item:", longest)
python list_report.py
1. bread
2. avocado
3. milk
4. sweet potatoes
5. tea
Items with more than 4 letters: 4
Longest item: sweet potatoes
plp-python-week7
│
├── list_warmup.py
├── shopping_list.py
├── list_report.py
├── README.md
└── screenshots
    ├── list_warmup.png
    ├── shopping_list.png
    └── list_report.png
# PLP Python Week 7 - Lists

## Files

- `list_warmup.py` - Demonstrates list indexing, append, remove, and len.
- `shopping_list.py` - Provides an interactive shopping list using add, remove, show, and done.
- `list_report.py` - Numbers items, counts item names with more than four letters, and finds the longest item.
- `screenshots/` - Contains screenshots showing each program running.

## Why is it safer to check `in` before calling `.remove()`?

It is safer to check `in` first because `.remove()` raises a ValueError if the item does not exist in the list. Checking with `in` allows the program to give a helpful message instead of crashing.
plp-python-week7
│
├── list_warmup.py
├── shopping_list.py
├── list_report.py
├── README.md
└── screenshots
    ├── list_warmup.png
    ├── shopping_list.png
    └── list_report.png
    https://github.com/YOUR-USERNAME/plp-python-week7
