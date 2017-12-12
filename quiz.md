1. The pitfall is that null is also considered an object, therefore a reliable way of avoiding this is to check if bar is null.
2. In the outter functions we’d get “bar” and in the inner we’d get “undefined” and “bar”, this is because “this” is refering to the function it’s currently on, the inner function does not have access to the variable foo that’s why it gives an undefined output.
3. In JavaScript it’s the way to declare private variables, along with creating a namespace to avoid conflict between modules.
4. It’d return an object, because it doesn’t matter if it’s an array (like you’d expect in other languages)or not, in JS it’s considered an object.
5. It’d returned undefined because Baz is defined AFTER the function bar, given this when we call this.baz, this will refer to the function and search for baz there, it’ll not look in the parent object.
6. Since fucntions always return true, however, since f was not defined, as it was only used in the if statement the instruction typeof f would return “undefined”, adding a string to a number gives us back a string so we’d have 1undefined.
7. The first string would give us a false, this is because it’d search for the string “ab” when compared to “(ab)”, the second one would give us true because it’d match all the strings that start with either “aa” or “bb”
8. Strict Mode is used to have more control and make your code more secure, it’ll change the syntaxis and will throw up exceptions instead of allowing the code to run, for example, not declaring a variable using strict mode will halt the code whereas using simple javascript will not.
9. var double = (i) => i =>{
   return i * 2);
};


11. As far as I understand the classical inheritance gives all the children the same properties but also a chance to change or delete those properties, in prototype inheritance it is impossible to delete a prototype defined property.
