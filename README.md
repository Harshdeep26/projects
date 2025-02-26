Spell Checker Using Trie

A spell checker verifies whether a word exists in a dictionary. If the word is not found, it suggests similar words based on prefixes.


Concepts Used:-
Trie Data Structure: A Trie (prefix tree) stores words efficiently. Each node represents a character, and words are stored in a hierarchical manner.
Insertion: Words are added letter by letter into the Trie.
Search: A word is checked in the Trie by following the stored characters.
Word Suggestions: If a word is not found, the program suggests words that start with the given prefix.

Key Components:-

Trie Node Structure:
Each node contains 26 children (for lowercase a-z).
A boolean flag indicates whether a word ends at a node.
Insert Function: Adds words to the Trie.
Search Function: Checks if a word exists.


Suggestion Function: Retrieves words with a common prefix.


How It Works:-
Insert words into the Trie when initializing the dictionary.

When the user enters a word:-
If the word exists, it's correctly spelled.
If the word does not exist, find words with a similar prefix and suggest alternatives.
Suggestions are generated recursively by traversing the Trie from the last matching letter of the prefix.
