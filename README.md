ITEM 1:
def alphabet_soup(text): ---> this function defines to arrange the character in order included in the text
    return ''.join(sorted(text)) --> this sorts the characters in the function to sort out the letters

print(alphabet_soup("hello"))  --> this function prints the alphabetically arranged character given with the word.
print(alphabet_soup("codingwithece")) --> this function prints the alphabetically arranged character given with the word.
print(alphabet_soup("hacker")) --> this function prints the alphabetically arranged character given with the word.

ITEM 2: 
def emotify(text): --> this will define the function to replace certain words with their given symbol
    emoticons = {
        "smile" : ":)" , ---> this action calls to change the word with the symbol that equates to it
        "grin" : ":D" , ---> this action calls to change the word with the symbol that equates to it
        "sad" : ":((", ---> this action calls to change the word with the symbol that equates to it
        "mad" : ">:(" ---> this action calls to change the word with the symbol that equates to it
    }

    words = text.split() --> this function will split words by default
    result = []

    for word in words:
        if word in emoticons: 
            result.append(emoticons[word]) --> this function will call the equivalent symbol for the word.
        else:
            result.append(word) --> this function will print as is, no emotify will be converted.  
    return ' '.join(result)
    
print (emotify("make me smile"))
print (emotify("make me grin"))
print (emotify("make me sad"))
print (emotify("make me mad"))

ITEM 3:
writeyourcodehere = [1,2,3,4,5,6] --> this creates a list of numbers that is stored in a  variable

first, *middle, last = writeyourcodehere --> *middle indicates that all the characters or numbers between the first and last will be included

print("first:", first)
print("middle:", middle)
print("last:", last)
