## **Date**
- Date of Note Creation: 2024-09-26
- Last Updated: 2024-11-15

---

## **Key Takeaways**

- **Variables**: Variables are **labels** that you can assign to values.
- **Data Types**: There are multiple data types:
	- **Sequence Type**:
		- **Strings**: A *string* is a series of characters. Anything inside quotes is     considered a string in Python. It can be single/double quotes. methods can be applied to strings.
			- **Methods**: A *method* is an action that python can perform on a piece of data. There are multiple ways to work with strings:
				- **Changing Case**: There are different types of methods that can be applied on pieces of data. For example: ***title() , upper() , lower()*** are all methods which can be used to change Case in a string. 
				- **f-strings**: The *f* is for *format*, because Python formats the string by replacing the name of any variable in braces with it's value. 
				- **Tabs and Newlines**: We can add a tab or a new line using \t , \n respectively. Note that this is a backward slash.
				- **Stripping Whitespaces**
					- **lstrip**: same as *rstrip* but removes whitespaces from left of the strings.
					- **rstrip**: whitespaces on the end of the strings can be stripped using *rstrip()* method. To strip permanently, associate the stripped value to the variable name. for example: variable = variable.rstrip() removes whitespaces permanentaly
				- **Removing Prefix/Suffix**: using *removeprefix() , removesuffix()* removes the defined prefix/suffix. To define prefix/suffix, write that particular part of the string in parenthesis('character') with single quotation.
	- **Numeric**:
		- **Numbers**: Python treats numbers in several ways, depending on how they're being used. Numbers consists of:
			- **Integers**: a number that is not a fraction; a whole number;
				- You can add (+), subtract (-), multiply (*), and divide (\) integers in python.
				- Python uses two multiplication symbols to represent exponents.
				- Python supports order of operations which can be modified by using parentheses. 
					- for example: 
						- $2+3 *4 = 14$
						- $(2+3)*4 = 20$
			- **Floats**: Any number with a decimal point are recognised as Floats.
				- for example:
					- $0.1 + 0.1 = 0.2$
					- $2*0.2 = 0.4$
			- **Integers and Floats**: If float is used in any operation, the result will contain a float.
				- for example:
					- $2+2=4$
					- $2+2.0=2.0$
			- **Underscores in Numbers**: Underscores can be used in python to group long numbers for organised and easier reading. The result is not affected and Python ignores the underscores.
				- for example: 
					 `>>>universe_age = 14_000_000_000`
					 `>>>print(universe_age)`
					 `14000000000`
- **Assignment**: 
	- **Multiple Assignment**: To shorten the codes length, multiple variables can be assigned multiple/single values to per variable
		- for example: 
			 `>>> x,y,z = 0,0,0`
			 `>>> y` 
			 `0`
			 `>>> x,y,z = 1,3,2`
			 `>>> y`
			 `3`
- **Constants**: Python does not recognise constants. Programmers mutually concluded that any variable named in capitals, would be recognised as a constant. WTF.
- **Comments**: a *comment* allows you to describe your **Approach** to the problem you're trying to solve. using # allows you to write comments. Anything following a hash-mark is ignored by python interpreter. It saves **Time!**. 
- **The Zen of Python**: This is a set of principles for writing good python code. This is to avoid complexity and to avoid complexity and aim for simplicity whenever possible.
	`Beautiful is better than ugly.`  
	`Explicit is better than implicit.`  
	`Simple is better than complex.`  
	`Complex is better than complicated.`  
	`Flat is better than nested.`  
	`Sparse is better than dense.`  
	`Readability counts.`  
	`Special cases aren't special enough to break the rules.`  
	`Although practicality beats purity.`  
	`Errors should never pass silently.`  
	`Unless explicitly silenced.`  
	`In the face of ambiguity, refuse the temptation to guess.`  
	`There should be one-- and preferably only one --obvious way to do it.`  
	`Although that way may not be obvious at first unless you're Dutch.`  
	`Now is better than never.`  
	`Although never is often better than *right* now.`  
	`If the implementation is hard to explain, it's a bad idea.`  
	`If the implementation is easy to explain, it may be a good idea.`  
	`Namespaces are one honking great idea -- let's do more of those!`
  This philosophy is for simplicity and clarity in mind.
---

## **Important Concepts**
### **Print Calls**
- **Description**: Print() has some defaults. 
- **Example**: while using print, double quotation is used to write anything that is not a command. 

---

## **Code Snippets**
### **Snippet 1:**
```python
# Using Format strings 
first_name = "ada"
last_name = "lovelace"
full_name = f"{first_name} {last_name}"
message = f"Hello, {full_name.title()}!"
print(message)

---
Hello, Ada Lovelace!
---
```

---
