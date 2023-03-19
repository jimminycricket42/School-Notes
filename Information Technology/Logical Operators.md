---
date: [Wed 25/05 2022]
aliases: [Boolean Logic ]
tags: [GR10/Q2 code/Logic]
modified: Thu 03/11 2022 08:00
---
# Logical Operators
- Not
- And
- Or 

## Not
**Values**: 0; 1
**Test**: Flip the values of the input, so true becomes false and false becomes true

## And
**Values**: 0; 1
**Test**: Do the two statements are both true. If they are true, then the and gate is true. If they are not true, the and gate is false. 
  

## Or
**Values**: 0; 1
**Test**: Are either of two statements true. If one is, then the gate is true. 

| B   | B   | A or B | Description                           |
| --- | --- | ------ | ------------------------------------- |
| 0   | 0   | 0      | False – both values are false         |
| 1   | 0   | 1      | True - One of the two values are true |
| 0   | 1   | 1      | True - One of the two values are true |
| 1   | 1   | 1      | True – Both values are true           |

## Order Of Expressions
1. Brackets
2. Not
3. And
4. Or

‘BNAO’ – Big Nate Ate Oats

## Truth Tables
Truth tables are a way of mapping all the possible combinations of a Logical Statement when we do not know the given values

For instance:
```Luhan is 20yrs old AND NOT(Swimming is on Fridays) ```

We do not know how old Luhan is, nor do we know when swimming is. So, we can plot this out to see when it would be true. In this case, let’s make ```Luhan is 20yrs old``` into variable ```A``` and make ```Swimming is on Fridays``` into variable ```B```. We can now express this as: ```A AND NOT B```
 
Now we can use a truth table to figure out when this statement will be true:

| A   | B   | Working     | Working | A AND NOT B | Result |
| --- | --- | ----------- | ------- | ----------- | ------ |
| 0   | 0   | 0 AND NOT 0 | 0 AND 1 | 0           | False  |
| 0   | 1   | 0 AND NOT 1 | 0 AND 0 | 0           | False  |
| 1   | 0   | 1 AND NOT 0 | 1 AND 1 | 1           | True   |
| 1   | 1   | 1 AND NOT 1 | 1 AND 0 | 0           | False  |

## Representing Logical Operators as Functions
- Or can be represented as ‘+’
- And can be represented as ‘·’
- Not can be represented as ‘'’

So, to represent logic A AND NOT B will be:

$$
f(A, B) = A·B'
$$
