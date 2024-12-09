## **Date**
- Date of Note Creation: 2024-09-27
- Last Updated: 2024-12-09

---

## **Key Takeaways**
- **What is a List?**
	- **Lists**: [[Lists]] come under [[Sequence Type]], a category of [[Data type]]. Indicated using squared brackets "[]" , elements are separated by commas. Lists are assigned to a label just like a variable.
	- **Accessing Elements in a list**: To access the element/s in the list, use the [[Variable]] name assigned to that list, followed by the index of the item enclosed in square brackets.
	 `my_list = ['apple', 'banana', 'cherry']`
	 `print(my_list[1]) # Output: banana`
	- **Index Position starts at 0, not 1**: Explains for itself but to remember, Index number for items in the list are off by 1. Also, to access the last item in the list, use negative indexing `my_list[-1]`. This will be beneficial when total number of items in the list is unknown.
	- **Using Individual Values from a List**: Pulling individual values from a list works the same way as *f-strings* do, which can be contained in *f-string* to compose another message. 
		- *for example*: `variable = f"message {my_list[3].title()}."`
- **Modifying, Adding and Removing Elements**
	- **Modifying Elements in a List**: To modify an item in list, use the name of the list followed by the index number of the element you want to change and then provide the new value you want that item number to have.
		- *for example*: `my_list[0] = 'new_item'` or 
		 `my_list = ['apple', 'banana', 'cherry'] 
		 `my_list[0] = 'orange' 
		 `print(my_list) # Output: ['orange', 'banana', 'cherry']`
	- **Adding Elements to a list**: Python provides several ways to add new data to existing lists.
		- **Appending Elements to the End of a list**: `my_list.append('new_item')`is the simplest way to add an item at the end of the list. Nothing else in the list gets affected. This can work even on empty lists! This is a common practice, programs which requires dynamic user data when program runs, use empty lists to begin with.
		- **Inserting Elements into a list**: `my_list.insert(0, 'new_item')` will add the `new_item` on the specified position in `my_list`. All the items on the right to newly inserted element, will shift by one position in the list.
			- *for example:* 
		     `my_list = ['apple', 'banana'] 
		     `my_list.insert(1, 'orange') 
			 `print(my_list) # Output: ['apple', 'orange', 'banana']`
	- **Removing Elements from a List**
		- **Removing an Item Using the del Statement**: `del my_list[2]` can be used when we know the index number of the element you want to delete in the list. This permanently deletes the element. `del` permanently deletes the item, and the value is lost.
		- **Removing an Item Using the pop() Method**: Just like del statement, `new_list = my_list.pop()`method removes the last element by default, but that element can be used as we remove it.`pop()` removes the item but allows you to use it afterward by **returning** when asked.
			- *for example:*
			 `my_list = ['apple', 'banana', 'cherry'] 
			 `my_list.pop(1) # Removes 'banana' 
			 `print(my_list) # Output: ['apple', 'cherry']`
			 
			 - `pop()` is particularly helpful in scenarios where you need to:
			1. Remove an item from a list.
			2. Process the removed item further.
			
		- **Removing an Item by Value**: `my_list.remove('useless_element')`is useful when the position of the item to be deleted is unknown, name of the value can be used as the key to remove it!
- **Organizing a List**
	- **Sorting a List Permanently with the sort() Method**: `my_list.sort()` is a nice way to sort a list in an alphabetical order. The change to a list is permanent and cannot be reverted to the original list. There's also a way to use `sort()` method to list elements in reverse-alphabetical order. To do so, pass the argument `reverse=True` to the `sort()` method.`my_list.sort(reverse=True)`
	- **Sorting a list Temporarily with the sorted() Function**: Unlike `sort()`method, which modifies the original list, `sorted(my_list)`does not change the original list. This is good in the cases where we do not want to affect the original list.
	- **Printing a List in Reverse Order**: In a case where you'd want to present the list in reverse order, `my_list.reverse()`method can be used. It does not care for the alphabetical arrangement instead, it reverses the order of the list. The changes are permanent but, can be reverted if applied twice.
	- **Finding the Length of a List**: `len(my_list)`function can be used to find the length of the list. The output is the total number of elements in the list.
- **Avoiding Index Errors When Working with Lists**
	- **Index Error**: Lists have a nature of off-by-one. This causes a common index error. Index error means Python can't find an item at the requested index.
	- **Negative Indexing**: To access the last item of the list, simply use `-1` as the index number while calling the element. `my_list[-1]`. Negative indexing counts from the end of the list, with `-1` being the last item, `-2` the second-to-last, and so on.

---

## **Important Concepts**
### **Concept 1: Adding and Removing Elements**

- **Description**: The most common operations with lists involve adding or removing items. Use `append()` to add items to the end of a list, `insert()` to place them at specific positions, and `pop()` or `remove()` to delete items.
- **Example**:
    `my_list = ['apple', 'banana'] 
	`my_list.append('cherry')  # Add to the end 
	`my_list.pop()  # Remove the last item`
	
---

### **Concept 2: Sorting Lists**

- **Description**: Lists can be sorted alphabetically or in reverse using `sort()` (permanent) or `sorted()` (temporary). Use `reverse()` to invert the order of elements.
- **Example**:
    `my_list = ['banana', 'apple', 'cherry'] 
    `my_list.sort()  # Sort permanently`

---
### **Concept 3: Using `pop()` to Return Values**

- **Description**: The `pop()` method not only removes an item from the list but also **returns its value**. This makes it useful when you need to process or store the removed item for later use, such as in task queues or interactive programs.
- **Example**:
    `tasks = ['task1', 'task2', 'task3']
	`# Remove and return the last task
	`current_task = tasks.pop()
	`print(f"Processing: {current_task}")  # Output: Processing: task3
	`print(tasks)  # Output: ['task1', 'task2']

---

## **Code Snippets**
### **Snippet 1: Add and Remove Items**
```python
# Description: Add and remove items in a list dynamically.
my_list = ['apple', 'banana']
my_list.append('cherry')  # Add to the end
my_list.pop(1)  # Remove by index
print(my_list)  # Output: ['apple', 'cherry']
```

### **Snippet 2: Organize a List**
```Python
# Description: Sort and reverse a list.
my_list = ['banana', 'apple', 'cherry']
print(sorted(my_list))  # Temporary alphabetical sort
my_list.reverse()       # Reverse the order
print(my_list)          # Output: ['cherry', 'apple', 'banana']
```

