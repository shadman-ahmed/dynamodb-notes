### Secondary Indexes
___
A secondary index enable to query the data in the table using an alternative key, in addition to queries using 
against primary key. Secondary indexes are optional.

Two types of indexes:
* **Global secondary index (GSI) -** An index with a partition key and sort key that can be different from those on 
  the table
* **Local secondary index (LSI) -** An index that has the same partition key as the table, but a different sort key

Each table has quota of:
- 20 global secondary index (default quota) 
- 5 local secondary index
