# Equality VS Identity

This blog explain difference between Equality(==) vs Identity(===)

In JavaScript, we have Equality (==) and Identity(===) operators for equality comparison between two values/operands. 
When first time we see Equality (==) and Identity (===) operators, then following questions arise in our mind. 

1. What is difference between Equality (==) and Identity (===) ? 
2. Is there a performance benefit with Equality (==) or Identity (===) ? 

Answers: 

1. What is Difference Between Equality (==) And Identity (===) ? Equality (==) returns true if both value/operands 
    have the same value, without worrying about type of both value/operands. 
    e.g.
    ```JavaScript
    2 == 1 // returns false, both value/operands have different value.
    2 == 2 // returns true, both value/operands have same type and value
    2 == "2" // returns true, while both value/operands have different type, first value is type of number and second one is type of string, but value is same.
    ```
    
    Equality (==) first compares types, if types are not same, then first convert both values/operands to same type, 
    then compare both value/operands, while on other hand Identity (===) first compares types, if types are same then 
    it only compares the value of both the operands, otherwise returns false.
    e.g.
    ```JavaScript
    2 === 1 // returns false, both value/operands have different value.
    2 === 2 // returns true, both value/operands have same type and value
    2 === "2" // returns false, both value/operands have same value but different types, first value is type of number and second one is string.
    ```

2. Is there a performance benefit with Equality (==) or Identity (===) ? 
    Identity (===) does not do type conversion (if types are not same it returns false), So Identity (===) is faster than Equality (==).
    
    > Identity (===), is generally better and safer, because there is no behind the scenes type conversion.

Follow Me
---
[Github](https://github.com/AmitThakkar)

[Twitter](https://twitter.com/amit_thakkar01)

[LinkedIn](https://in.linkedin.com/in/amitthakkar01)

[More Blogs By Me](http://amitthakkar.github.io/)