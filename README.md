# ECE2112 Programming Problems

This repository contains Python scripts for solving various programming problems in ECE2112. Below is an overview of each script included.

### 1. Alphabet Soup Problem

**Function:**

```python

# Define a function that takes a string as an input and returns a new string
def alphabet_soup(word):
    # Convert the string first into a list of characters
    char_list = list(word)
    # Then, sort the list alphabetically
    char_list.sort()
    # Join the sorted characters back into a string
    sorted_word = ''.join(char_list)
    return sorted_word

# Sample text to test the function
result = alphabet_soup("doscutie")

# Print the result to see the output
print(result)

```

**Output:**
'cdeiostu'



### 2. Emoticon Problem

**Function:**

```python

# Define a function that replaces specific words in a text with their corresponding emoticons
def emoticon(sentence):
    # Define a dictionary where words are the keys and the emoticons that go with them are the values.
    replacements = {
        "smile": ":)",   # smile is replaced with :)
        "grin": ":D",    # grin is replaced with :D
        "sad": ":((",    # sad is replaced with :((
        "mad": ">:("     # mad is replaced with >:(
    }
    
    # Loop through the dictionary and replace each word in the sentence with its emoticon
    for word, emoticon in replacements.items():
        # Replace occurrences of the word in the sentence with the corresponding emoticon
        sentence = sentence.replace(word, emoticon)

    # Return the modified sentence with the words replaced by their respective emoticons
    return sentence
    
# Sample sentence to test the function
sentence = "Do not be sad and mad, I love seeing you smile and grin."

# Call the function with the sample text and store the result
result = emoticon(sentence)

# Print the result to see the output
print(result)

```

**Output:**
'Do not be :(( and >:(, I love seeing you :) and :D.'



### 3. Unpacking List Problem

**Function:**

```python

# Given list containing a sequence of numbers
writeyourcodehere = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Unpack the list into three parts:
# 'first' gets the first element of the list,
# 'middle' captures all elements between the first and last as a list,
# 'last' gets the final element of the list.
first, *middle, last = writeyourcodehere

# Print the result
print("First:", first)   
print("Middle:", middle) 
print("Last:", last)

```

**Output:**
'First: 1, Middle: [2, 3, 4, 5, 6, 7, 8, 9], Last: 10'
