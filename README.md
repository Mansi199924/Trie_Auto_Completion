# Trie_Auto_Completion
# What is Trie data structure?
A trie is a tree-like information retrieval data structure whose nodes store the letters of an alphabet. It is used to store the key . Main advantage of trie is searching a particular key . This can be done be in O( length_of_key ) which is very fast in compare to naive search where we check for every word in our collections that it matches with key.

# Auto Completion using Trie
We are given a Trie with a set of strings stored in it. Now the user types in a prefix of his search query, we need to give him all recommendations to auto-complete his query based on the strings stored in the Trie.
For example if the Trie store {“abc”, “abcd”, “aa”, “abbbaba”} and the user types in “ab” then he must be shown with this {“abc”, “abcd”, “abbbaba”}.

We can store all the words which are most used or which are most typed by user in past . Now whenever user types a prefix , our algorithm will find all suggestion ( or words ) which user actually want to type.
All utility function (like searching ,addition , deletion , auto_complete ) are implemented in C++.

We can modify our "trienode structure" to store frequency of word . Every time a word is suggested( user used this suggestion ) or user typed it himself we increase this frequency variable . This frequency variable help us to suggest most frequent word to user. We can modify structure to hold all letter ( A-Z , a-z ).
