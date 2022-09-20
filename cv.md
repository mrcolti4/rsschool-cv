# Kyrylo Bulyhin
## JavaScript/Front-end 2022Q3 student
### My contacts 
* Location: Zaporizhya, Ukraine
* Phone: +380 663 168 308
* E-mail: kbulygin456@gmail.com
### About me
I got acquainted with programming in 2019, then I just started my journey learning HTML and CSS from the book "The New Big Book of CSS" by David Sawyer McFarland and McFarland David. Having created a couple of simple websites, I realized that I wanted to create not just a layout, but something more and decided to learn a real programming language. I chose Python as my first language because it was on the rise. And later I got acquainted with his most popular framework - Django.

In these courses from rs school, I expect to advance in my knowledge of markup and Java Script language in order to become a professional developer later
### Skills 
* HTML5, CSS
* JS Basics
* Python, Python Django basics
* Git, GitHub
* AdobePhotoshop, Figma
* Neovim, VS Code, Intellij IDEA
### Code Examples
On the CodeWars site, I performed tasks for both Python and JavaScript. Here are some examples of tasks.
*Credit Card Mask*: Usually when you buy something, you're asked whether your credit card number, phone number or answer to your most secret question is still correct. However, since someone could look over your shoulder, you don't want that shown on your screen. Instead, we mask it.
Your task is to write a function *maskify*, which changes all but the last four characters into *'#'*.
``` javascript
function maskify(cc) {
    let result, ccLength, lastFourChars;
    ccLength = cc.length;
    if (ccLength > 4) {
        lastFourChars = cc.slice(ccLength-4);
        result = `${'#'.repeat(ccLength - 4)}${lastFourChars}`;
        return result;
    } else {
        return cc;
    }
}
```

*First non-repeating character*: Write a function named *first_non_repeating_letter* that takes a string input, and returns the first character that is not repeated anywhere in the string.

For example, if given the input *'stress'*, the function should return *'t'*, since the letter t only occurs once in the string, and occurs first in the string.

As an added challenge, upper- and lowercase letters are considered the same character, but the function should return the correct case for the initial letter. For example, the input *'sTreSS'* should return *'T'*.

If a string contains all repeating characters, it should return an empty string ("") or *None* -- see sample tests.
``` Python
from collections import Counter

def first_non_repeating_letter(string):
    counter = Counter(string.lower())
    result = [i.upper() if i.upper() in string else i.lower() for i in counter if counter[i] == 1]
    return result[0] if result else ''
```