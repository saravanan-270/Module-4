# Exp.No:18  
## FILES - FREQUENCY OF CHARACTERS IN A FILE

---

### AIM  
To write a Python program that reads a file and counts the frequency of each character in it.

---

### ALGORITHM

1. Begin the program.  
2. Define the function `create_file()` that accepts two arguments:  
   - `file_path`: The path to the file.  
   - `content`: The string content to be written into the file.  
3. Open the file specified by `file_path` in write mode (`'w'`), and write the provided `content` into the file.  
4. Close the file (this is automatically done when exiting the `with` block).  
5. Define the function `character_frequency()` that accepts one argument:  
   - `file_path`: The path to the file whose character frequency is to be calculated.  
6. Open the file specified by `file_path` in read mode (`'r'`), and read its content into the variable `content`.  
7. Initialize an empty dictionary (`d1`) to store the frequency of each character using `defaultdict(int)`.  
8. Loop through each character in the `content`:  
   - For each character `ch`, increment its corresponding frequency in the dictionary `d1`.  
9. Return the dictionary `d1`, which contains the frequency of each character in the file.  
10. Terminate the program.

---

### PROGRAM

```
from collections import defaultdict

def create_file(file_path, file_content):
    with open(file_path, 'w') as file:
        file.write(file_content)

def char_frequency(file_path):
    with open(file_path, 'r') as file:
        content = file.read()
    
    frequency = defaultdict(int)  # Initialize a defaultdict to count character frequencies

    for char in content:
        frequency[char] += 1  # Increment the count for each character

    return frequency

# Example usage
file_path = 'example.txt'

# Test case 1
file_content_1 = "saveetha engineering college"
create_file(file_path, file_content_1)
# print("Character frequencies:", char_frequency(file_path))

# Test case 2
file_content_2 = "computer science engineering"
create_file(file_path, file_content_2)
# print("Character frequencies:", char_frequency(file_path))
```


### OUTPUT
![image](https://github.com/user-attachments/assets/341d6e48-865f-4f34-b1d0-725be2427345)


### RESULT
Thus a Python program that reads a file and counts the frequency of each character in it was implemented and executed successfully.
