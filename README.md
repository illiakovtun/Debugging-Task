1. Issue was an error, where we were missing one IDs of POS.
2. To fix this problem I've removed null ID from list.
3. The root cause was: in out function we are comparing filtered and default array;
to make them similar we need to remove null ID
