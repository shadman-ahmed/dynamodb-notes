## Core Components
___
**Tables:** A table is a collection data (items) 

```
      table       item
        |         /    
personTable: [person1, person2, person3]
```
___
**Items:** An item is a group of attributes that is uniquely identifiable among other items.
In the example below, individual item is being uniquely identified by their name

```
personTable: [{
    person1: {
        name: person1,
        attribute2: attributeValue,
        attribute3: attributeValue,
    },
    person2: {
        name: person2,
        attribute2: attributeValue,
        attributeDifferent: attributeValue,
    },
    person3: {
        name: person3,
        attributeRandom: attributeValue,
        nestedAttribute: {
            nestedAttribute1: attributeValue,
            nestedAttribute2: attributeValue
        }
    },
}]
```
___
**Attributes:** An attribute is a fundamental data element which doesn't need further break down. 
DynamoDB supports nested attribute upto 32 level deep

```
exampleItem: {
        name: person3,
        attributeRandom: attributeValue,
        nestedAttribute: {
            nestedAttribute1: attributeValue,
            nestedAttribute2: attributeValue
        }
    },
```

**Next:** [Primary Key](primary-key.md)
<br/>
**Previous:** [Introduction](introduction.md)
