1. Issue was an error, where we were missing one IDs of POS.
2. To fix this problem I've replaced names of instances and results arrays.
3. The root cause was: Firstly we get results by reduce method and then use filter to get rid of 
pos_id that was previously null. After that to compare two arrays we use wrong variables.
