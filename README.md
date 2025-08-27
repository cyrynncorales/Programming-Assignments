# 🐍 PROGRAMMING ASSIGNMENTS USING PYTHON

This README explains three Python code snippets that demonstrate different functionalities:
- Sorting characters alphabetically
- Replacing words with emoticons
- Unpacking elements from a list

---

## 📌 ITEM 1: Alphabet Soup

```python
def alphabet_soup(text):  # This function arranges the characters in alphabetical order from the input text
    return ''.join(sorted(text))  # This sorts and joins the characters to form the alphabetized string

print(alphabet_soup("hello"))  # This prints the alphabetically arranged characters of the word
print(alphabet_soup("codingwithece"))  # This prints the alphabetically arranged characters of the word
print(alphabet_soup("hacker"))  # This prints the alphabetically arranged characters of the word
```

---

## 📌 ITEM 2: Emotify

```python
def emotify(text):  # This function replaces specific words with their corresponding emoticon symbols
    emoticons = {
        "smile": ":)",   # This maps the word to the smiley face symbol
        "grin": ":D",    # This maps the word to the grinning face symbol
        "sad": ":((",    # This maps the word to the sad face symbol
        "mad": ">:("     # This maps the word to the angry face symbol
    }

    words = text.split()  # This splits the input text into individual words
    result = []

    for word in words:
        if word in emoticons:
            result.append(emoticons[word])  # This replaces the word with its corresponding symbol
        else:
            result.append(word)  # This keeps the word unchanged if there's no matching emoticon

    return ' '.join(result)

print(emotify("make me smile"))
print(emotify("make me grin"))
print(emotify("make me sad"))
print(emotify("make me mad"))
```

---

## 📌 ITEM 3: List Unpacking

```python
writeyourcodehere = [1, 2, 3, 4, 5, 6]  # This creates a list of numbers stored in a variable

first, *middle, last = writeyourcodehere  # *middle collects all elements between the first and last

print("first:", first)
print("middle:", middle)
print("last:", last)
```

---
