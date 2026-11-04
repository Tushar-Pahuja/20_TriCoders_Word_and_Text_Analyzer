# Word and Text Analyzer

## C Programming Mini Hackathon

**Team Name:** TriCoders  
**Batch:** 20

### Team Members

| Name | SAP ID |
|---|---|
| Tushar Pahuja | 590032177 |
| Chahat | 590032461 |
| Pratham | 590032424 |

---

## Problem Statement

Develop a text analysis tool that processes a sentence entered by the user.

The program analyzes the entered text and generates useful statistics. It also checks whether the entered word or sentence is a palindrome while ignoring spaces and letter case where appropriate.

---

## Objectives

The main objectives of the project are:

- To develop a text analysis program using C.
- To count characters and words in a sentence.
- To count vowels and consonants.
- To identify the longest word.
- To check whether a word or sentence is a palindrome.
- To correctly handle empty input and multiple spaces.
- To apply fundamental C programming concepts to a practical problem.

---

## Features

The Word and Text Analyzer provides the following features:

- Character counting
- Word counting
- Vowel counting
- Consonant counting
- Longest word identification
- Palindrome checking
- Case-insensitive palindrome checking
- Space handling
- Empty input validation
- Menu-driven interface

---

## Program Menu

The program provides the following menu:

```text
========================================
          WORD & TEXT ANALYZER
========================================
1. Analyze Text
2. Check Palindrome
3. Exit
========================================
```

### Option 1: Analyze Text

Accepts a sentence and displays a complete text statistics report.

### Option 2: Check Palindrome

Checks whether the entered word or sentence is a palindrome while ignoring spaces and letter case.

### Option 3: Exit

Terminates the program.

---

## Algorithm / Pseudocode

```text
START

Display the main menu

Ask the user to select an option

IF option = Analyze Text

    Read the complete sentence

    IF input is empty or contains only spaces
        Display an error message
    ELSE
        Count characters
        Count words
        Count vowels
        Count consonants
        Find the longest word
        Check whether the sentence is a palindrome
        Display the text statistics report
    END IF

ELSE IF option = Check Palindrome

    Read a word or sentence

    IF input is empty or contains only spaces
        Display an error message
    ELSE
        Ignore spaces
        Ignore uppercase/lowercase differences
        Compare characters from beginning and end

        IF all corresponding characters match
            Display "Palindrome"
        ELSE
            Display "Not Palindrome"
        END IF
    END IF

ELSE IF option = Exit

    Terminate the program

ELSE

    Display "Invalid Choice"

END IF

STOP
```

---

## C Programming Concepts Used

The project uses the following C programming concepts:

- Variables and data types
- Character arrays and strings
- Functions
- Loops
- Conditional statements
- `switch` statement
- Arrays
- String handling
- Input validation
- Standard library functions
- Character handling functions

### Header Files Used

```c
#include <stdio.h>
#include <string.h>
#include <ctype.h>
```

---

## Main Functions

The program is divided into multiple functions:

```text
countCharacters()   - Counts the characters in the text
countWords()        - Counts the words
countVowels()       - Counts vowels
countConsonants()   - Counts consonants
findLongestWord()   - Finds the longest word
isEmpty()           - Checks for empty/space-only input
checkPalindrome()   - Checks whether the text is a palindrome
```

---

## Compilation and Execution

### Using GCC

Compile the program using:

```bash
gcc word_text_analyzer.c -o analyzer
```

Run on Windows using:

```bash
analyzer.exe
```

The program can also be compiled and executed using a C-supported IDE such as Visual Studio Code with GCC configured.

---

## Sample Test Cases

### Test Case 1 — Normal Input

**Input:**

```text
Hello World
```

**Expected Result:**

```text
Characters      : 11
Words           : 2
Vowels          : 3
Consonants      : 7
Longest Word    : Hello
Palindrome      : NO
```

---

### Test Case 2 — Palindrome Sentence

**Input:**

```text
Never odd or even
```

**Expected Result:**

```text
Palindrome: YES
```

---

### Test Case 3 — Mixed Case Palindrome

**Input:**

```text
Madam
```

**Expected Result:**

```text
Palindrome: YES
```

---

### Test Case 4 — Multiple Spaces

**Input:**

```text
Hello     World
```

**Expected Result:**

```text
Words: 2
```

The program correctly handles multiple spaces without counting them as additional words.

---

### Test Case 5 — Empty Input

**Input:**

```text
[No text entered]
```

**Expected Result:**

```text
Error: Input cannot be empty!
```

---

## Team Contribution

### Tushar Pahuja
- Input handling
- Character counting
- Word counting

### Chahat
- Vowel counting
- Consonant counting
- Longest word identification

### Pratham
- Palindrome checking
- Input validation
- Testing and menu handling

All team members participated in understanding, testing, integration, and presentation of the complete program.

---

## Conclusion

The Word and Text Analyzer successfully analyzes user-entered text and generates useful statistics such as character count, word count, vowel count, consonant count, and the longest word. It also checks whether a word or sentence is a palindrome while handling spaces and letter case appropriately.

This project demonstrates the practical application of fundamental C programming concepts including strings, arrays, loops, conditional statements, functions, and input validation.
