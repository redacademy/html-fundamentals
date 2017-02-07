# Coercion
Where there are different data types, one data type will be changed to an 'equivalent value '
of the other data type

Use strict equality operators (=== !==) to ensure the values converted are equaled
to avoid causing error


```javascript
1 +'2'; //12

if (0 && null) {
    console.log('we will not get here')
} ; //false

if (1 === '1') {
    console.log('we will not get here')
} ; //false 

if (null || (4 === 1 + 3) ){
    console.log('we will get here');  
}; // true
 

