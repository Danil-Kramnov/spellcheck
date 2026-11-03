Observations:
1. the document words are stored in a HashSet, so each unique word is checked only once
2. the misspelt count is 2796 using LinkedList
3. Dictionary size: 122790 (LinkedList)
4. misspelt count and n the same for ArrayList
5. LinkedList vs ArrayList: ArrayList access is faster compared to LinkedList one due to the fact that slots with references for ArrayList sits next to each other, just in one big array and CPU can prefetch around 16 references at once. But for LinkedList CPU should know the reference of the next slot based on previous slot, slots are linked (hence the name LinkedList). So here's an extra time for extra step/hop in case of LinkedList.
6. binarySearch works only on sorted array, but much faster method then contains due to lesser complexity. O(log(n)) vs O(n). 
7. 