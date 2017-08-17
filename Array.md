### Complexity
- Acess: O(1)
- Search: O(n)
- Insert: O(n)
- Space: O(n)

In java and .Net expanding an Array needs to recreate it. But in dynamic languages like Python its ok! To solve this problem, .Net and Java have List<> and ArrayList that are editable in size.

If the array is sorted in a way that's amenable to binary search, then you can search the array that way and achieve in the best case, array search is O(log n).
