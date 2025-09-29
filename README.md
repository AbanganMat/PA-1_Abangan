# Experiment 1 

# I. Intended Learning Outcomes:
1. To identify the basic codes and functions in Python Programming
2. To be able to apply the different codes and functions in creating a Python program,

# II. Instructions:
Write a Python script/code in the Jupyter Notebook to do the given problems. You may submit your Jupyter
notebook in the dedicated submission bin.

# ALPHABET SOUP PROBLEM
```
Define function
def alphabet(string):
    # Sort Characters
    char_list = list(string)

    # Sort in Alphabetical Order
    sorted_list = sorted(char_list)

    # Join into a single string
    sorted_string = "".join(sorted_list)

    # Return Sorted String
    return sorted_string

# Output
print(alphabet("iamlightningspeed"))
print(alphabet("supercalifragilisticexpialidocious"))
```
# EMOTICON PROBLEM
```
Define function
def emotify(sentence):
    # Mapping words to emoticons
    mapping = {
        "smile": ":)",
        "grin": ":D",
        "sad": ":(",
        "mad": ">:("
    }
    
    # Split sentence into pieces
    words = sentence.split()
    
    # Empty list to store converted words
    converted = []
    
    # Loop through each word
    for w in words:
        if w in mapping:
            converted.append(mapping[w])  # replace with emoticon
        else:
            converted.append(w)  # keep original sentence
    
    # Return the final string
    return " ".join(converted)

# Output
print(emotify("Make me smile but at the same time, make me sad"))
print(emotify("Currently feeling sad but I smile like never happened"))
print(emotify("smile until the end and grin like a man, carry on"))
```
# Unpacking List Problem
```
# Define function
def unpack_list(lst):
    # Get first element
    first = lst[0]

    # Get last element (count length and subtract 1)
    last = lst[len(lst) - 1]

    # Get middle elements (everything except first and last)
    middle = lst[1:len(lst)-1]

    # Return results
    return first, middle, last

# Example usage
numbers = [1, 2, 3, 4, 5, 6]
first, middle, last = unpack_list(numbers)

# Output
print("first:", first)
print("middle:", middle)
print("last:", last)
