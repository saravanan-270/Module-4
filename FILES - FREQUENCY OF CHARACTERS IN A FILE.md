# Exp.No:18  
## FILES - FREQUENCY OF CHARACTERS IN A FILE

---

### AIM  
To write a Python program that reads a file and counts the frequency of each character in it.

---

### ALGORITHM

1. Start the program.

Define the function create_file(file_path, file_content):

Step 2.1: Open the file specified by file_path in write mode ('w') using the open() function.

Step 2.2: Write the string file_content into the file using the write() method.

Step 2.3: Close the file automatically when exiting the function.

Define the function count_words_in_file(file_path):

Step 3.1: Open the file specified by file_path in read mode ('r') using the open() function.

Step 3.2: Read the entire content of the file and store it in a variable t.

Step 3.3: Split the string t into a list of words using the split(" ") function (which splits words by spaces).

Step 3.4: Count the total number of words by finding the length of the list using len(l).

Step 3.5: Return this word count as the result.

In the main program:

Step 4.1: Call the create_file() function to create a file and write the content into it.

Step 4.2: Call the count_words_in_file() function and pass the same file path to get the total word count.

Step 4.3: Display the number of words in the file.

End the program.

---
### PROGRAM

```python
def create_file(file_path,file_content):
    f=open(file_path,'w')
    f.write(file_content)
def count_words_in_file(file_path):
    f=open(file_path,'r')
    t=f.read()
    l=t.split(" ")
    return(len(l))

```


### OUTPUT

![WhatsApp Image 2025-10-28 at 14 45 11_a5ad13f2](https://github.com/user-attachments/assets/6413426c-76dd-4d3b-83d1-6563202cbdeb)

### RESULT
Thus the python program for that reads a file and counts the frequency of each character in it has been implemented and executed successfully.
