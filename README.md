# Lexical-Analyzer

This code defines a **LexicalAnalyzer** class that has several methods for tokenizing an expression and classifying the tokens as either NUMBER, IDENTIFIER, or SYMBOL.

The **return_token** method takes an expression as input and splits it into a list of tokens using a loop that scans the expression character by character. 
It groups the characters into tokens based on whitespace and certain symbols (+, -, *, /, (, ), and =).

The method then uses regular expressions to classify the tokens as either NUMBER, IDENTIFIER, or SYMBOL. A NUMBER token is a sequence of one or more digits. 
An IDENTIFIER token is a sequence of one or more letters, underscores, or digits that starts with a letter or underscore. 
All other tokens are classified as SYMBOL.

The method returns a list of tuples, each containing a tag and the corresponding token value.

The **takeinput** method prompts the user to enter an expression, and returns the expression as a string.

Finally, the code creates an instance of the **LexicalAnalyzer** class, prompts the user to enter an expression, tokenizes the expression, and prints the resulting list of tokens to the console.
For example, if the user enters the expression "a + b", the output will be:

[('IDENTIFIER', 'a'), ('SYMBOL', '+'), ('IDENTIFIER', 'b')]
