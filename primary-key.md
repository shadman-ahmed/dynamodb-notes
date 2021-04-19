### Primary Key
___
DynamoDB supports two kind of primary key

1. **Simple primary key** - Partition key
2. **Composite primary key** - Partition key and sort key

**Simple primary key:** When only one attribute is used as the partition key/hash attribute. In a table that has 
only one partition key, no two items can have the same partition key.

**Composite primary key:** A composite primary is composed of two attributes. The first attribute is the partition 
key, and the second attribute is the sort key. In a table with composite primary key, two items can have same 
partition key value, but those two items must have different sort key values. 

**Note:** 
* For both **simple primary key** and **composite primary key**, the partition key value is used as the input 
of an internal hashing function. The output of the internal hash function determines the actual physical address of 
the partition (internal storage) where the item will be stored. 
  
* In a table with **composite primary key**, all items with same partition key value are stored physically together, in sorted oder by sort key value
  
* **Composite primary key** enables to query a subset of items from a table based on their partition key value

* Partition key and sort key are also known as hash attribute and range attribute respectively 


**Next:** [Secondary Indexes](secondary-index.md)
<br/>
**Previous:** [Introduction](core-components.md)

