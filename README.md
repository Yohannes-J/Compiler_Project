#Assignment: Compiler Design using Swift
# Group 8

| Number |         Name          |    ID    |
|--------|-----------------------|----------|
| 1      |  Ashenafi Minaye      | 1300403  |
| 2      |  Bethelihem Asmiro    | 1306222  |
| 3      | Endale Gebeyehu       |  1301039 |
| 4      |  Kedir Tahir          |  1301743 |
| 5      | Yohannes Alemayehu    | 1303096  |

Project Title: Design And Implementation Of A Lexical Analayzer for Swift Language.

#A lexical analyzer (also called a lexer or scanner) is a program or part of a compiler that performs lexical analysis.
Its primary role is to take a stream of characters (such as source code in a programming language) and convert it into a sequence of tokens.
These tokens are then used by the compiler or interpreter for further processing, such as syntax analysis.
Input: The lexical analyzer takes raw text input, typically the source code of a program written in a programming language.
Output: It produces a sequence of tokens, each representing a meaningful unit in the language,
such as keywords, identifiers, operators, literals, punctuation, etc.
Token: A token is a categorized block of text, often consisting of a type (such as keyword, identifier, number, etc.) 
and its associated value (such as a variable name or a literal value).
Regular Expressions: Lexical analyzers often use regular expressions to define the patterns for different types of tokens.
in our project we are the swift sample code and lex file that identify available tokens in the swift code by token type, 
values of token and line number in tabular form. 
Example:
For a simple code :
Copy
int x = 10;
The lexical analyzer would break it into tokens:
int (Keyword)
x (Identifier)
= (Operator)
10 (Integer Literal)
; (Semicolon)


#INSTRUCTIONS: to run this file download the zip file from here and extract where you want and remove the c and lexer file.
open extracted file in command promt.
run flex swift_lex.l file,
gcc lex.yy.c -o lexer
lexer inputCode.swift
expected output is like this...
 Token Type           | Value       | Line Number|
|---------------|-------------|------------------|
| KEYWORD            | var          | 1          |
| IDENTIFIER         | sum          | 1          |
| UNKNOWN EXPRESSION | =            | 1          |
| DIGIT              | 0            | 1          |
| KEYWORD            | var          | 2          |


