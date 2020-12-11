1. Issue was an error, where we were missing one IDs of POS.
2. To fix this problem I've replaced filtered array with our default results array.
3. The root cause was: Firstly we get results by reduce method but then use filter to get rid of 
pos_id that was previously null.
