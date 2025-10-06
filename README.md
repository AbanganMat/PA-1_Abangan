# Experiment 1 - Abangan

# I. Intended Learning Outcomes:
1. To identify the basic codes and functions in Python Programming
2. To be able to apply the different codes and functions in creating a Python program,

# II. Instructions:
Write a Python script/code in the Jupyter Notebook to do the given problems. You may submit your Jupyter
notebook in the dedicated submission bin.

# ALPHABET SOUP PROBLEM
```
# Define a function named 'alphabet' that takes one input: string
def alphabet(string):
    # Convert the string into a list of characters
    char_list = list(string)

    # Sort the list of characters in alphabetical order
    sorted_list = sorted(char_list)

    # Join the sorted characters back into a single string
    sorted_string = "".join(sorted_list)

    # Return the sorted string
    return sorted_string

# Test the function with two examples and print the results
print(alphabet("iamlightningspeed"))
print(alphabet("supercalifragilisticexpialidocious"))
```
<img width="275" height="41" alt="Screenshot 2025-10-06 at 08 43 25" src="https://github.com/user-attachments/assets/eb0c5c7f-2a61-4655-913f-f7bbc686e6dc" />

# EMOTICON PROBLEM
```
# Define a function named 'emotify' that takes one input: sentence
def emotify(sentence):
    # A dictionary that maps certain words to their corresponding emoticons
    mapping = {
        "smile": ":)",
        "grin": ":D",
        "sad": ":(",
        "mad": ">:("
    }
    
    # Split the sentence into individual words
    words = sentence.split()
    
    # Create an empty list to store the converted words
    converted = []
    
    # Go through each word in the sentence
    for w in words:
        # If the word is in the mapping dictionary, replace it with an emoticon
        if w in mapping:
            converted.append(mapping[w])
        # Otherwise, keep the original word
        else:
            converted.append(w)
    
    # Join all the words (and emoticons) back into a single string
    return " ".join(converted)

# Test the function with example sentences
print(emotify("Make me smile but at the same time, make me sad"))
print(emotify("Currently feeling sad but I smile like never happened"))
print(emotify("smile until the end and grin like a man, carry on"))
```
<img width="392" height="51" alt="Screenshot 2025-10-06 at 08 43 34" src="https://github.com/user-attachments/assets/8db718ee-9915-4633-89e3-6c8948494510" />

# Unpacking List Problem
```
# Define a function named 'unpack_list' that takes one input: lst (a list)
def unpack_list(lst):
    # Get the first element of the list
    first = lst[0]

    # Get the last element of the list using its length
    last = lst[len(lst) - 1]

    # Get all the middle elements (everything except the first and last)
    middle = lst[1:len(lst)-1]

    # Return the three parts: first, middle, and last
    return first, middle, last

# Example list to test the function
numbers = [1, 2, 3, 4, 5, 6]

# Call the function and store the returned values
first, middle, last = unpack_list(numbers)

# Display the results
print("first:", first)
print("middle:", middle)
print("last:", last)
```
<img width="163" height="51" alt="Screenshot 2025-10-06 at 08 43 42" src="https://github.com/user-attachments/assets/8a7abdb0-cbd6-4a5b-ada5-c42efad778bf" />
