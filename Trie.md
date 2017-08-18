# Trie
- Lookup: **O(m)** in worse case where **m** is length of search string
- Space: In worse case it will be **O(m*n)** which **m** is length of longest string and **n** is number of words in th trie.

Trie is an efficient information retrieval data structure. Using trie, search complexities can be brought to optimal limit (key length). If we store keys in binary search tree, a well balanced BST will need time proportional to M * log N, where M is maximum string length and N is number of keys in tree. Using trie, we can search the key in O(M) time. However the penalty is on trie storage requirements. [source](http://www.geeksforgeeks.org/trie-insert-and-search/)

## Examples
- AutoComplete (The most common scenario)
- Search in Contact List
- Spell checker
- T9 predictive text
- Solving word games


## Implementation

- Java Implementation With Array ([source](source/TrieImplementationWithJava.java))
Implementation with array resault in faster insert because there is no need to expand ArrayList or HashMap which have its Complexity (in worse case O(n)).But, it just works if we have a specific range of characters. For example if your do not know language of the text to be indexed therefore, you should use HashMap implementation
```Java
class TrieNode {
    TrieNode[] arr;
    boolean isEnd;
    // Initialize your data structure here.
    public TrieNode() {
        this.arr = new TrieNode[26];
    }
 
}

public class Trie {
    private TrieNode root; 
    ...
```

- Java Implementation With HashMap ([source](TrieIMplementationWithList))

```Java
// Inserts a word into the trie.
    public void insert(String word) {
        HashMap<Character, TrieNode> children = root.children;
 
        for(int i=0; i<word.length(); i++){
            char c = word.charAt(i);
 
            TrieNode t;
            if(children.containsKey(c)){
                    t = children.get(c);
...
```

- C# Implementation With Dictionary ([source](https://gist.github.com/benyblack/23cfeda6772b3d54c69139d4d2064604))
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
namespace MyTrie {
    public class TrieNode {
        Dictionary<char, TrieNode> children = new Dictionary<char, TrieNode>();
        public int Size { get; set; }

        public TrieNode() {
            Size = 0;
        }

        private TrieNode GetNode(char c) {
            if (children.ContainsKey(c)) {
...
```