<h1>Mod 2 Week 1 Review</h1>
<p>In this document there will be explainations of common array and object prototype and 'this' context examples.</p>
<h2>Array.concat()</h2>
<p>In this example, there are two arrays (fruits and vegetables).</p>
<p>In the change function, we are returning the output of fruits.concat.vegetables.</p>
<ul>
  <li>fruits is the first array</li>
  <li>.concat is the prototype</li>
  <li>vegetables is the second array</li>
</ul>
<h3>arr.concat concatenates both arrays into one array.</h3>
<p>The result, on the right side, combines both arrays:</p>
<p>[ 'apple', 'orange', 'banana', 'berries', 'lime', 'lemon', 'mango', 'pear', 'mushroom', 'onion', 'garlic', 'broccoli']</p>
<img src="images/Array Prototypes/arr.concat Example.png" alt="Array Prototype Concat">
<h2>Array.copyWithin()</h2>
<p>In this example, there is one array (foods).</p>
<p>In the change function, we are returning the output of foods.copyWithin(5,1).</p>
<h3>foods.copyWithin makes a copy of some elements in the array and replaces other elements in the array with those copied elements.</h3>
<p>There are also two numbers attached to foods.copyWithin.</p>
<p>In this case, 5 states the index number of the first element that should be replaced.</p>
<p>1 states the index number of the first element to be copied that will replace the original element at index 5.</p>
<p>In this example, the element at index 1 and anything afterwards (equivalent to the number of elements after index 5(inclusive of index 5)) will be copied.</p>
<p>That is to say, if there are only 6 indexes in the array,  5 and 6 will be replaced.</p>
<p>If we are starting at index 1, only index 1 and index 2 will be copied to replace index 5 and index 6.</p>
<p>The result can be seen in the console.</p>
<p>[ 'apple', 'orange', 'banana', 'berries', 'lime', 'orange', 'banana', 'berries']</p>
<img src="images/Array Prototypes/arr.copyWithin Example.png" alt="Array Prototype copyWithin">
<h2>Array.every()</h2>
<p>In this example, there is one array (fruits).</p>
<p>There are two functions, yum and change.</p>
<p>In the yum function, we are passing in the fruits array and returning the 12th index of fruits (Hint: There is no 12th index).</p>
<h3>array.every returns true or false depending if all the elements in the array pass the test provided in the function.</h3>
<p>In the yum function, we are checking for the 12th element.</p>
<p>In the change function, we are returning the output of the fruits array after checking every element to see if it mathces the conditions in the yum function.</p>
<p>Since there is no 12th index, the return is false.</p>
<img src="images/Array Prototypes/arr.every Example.png" alt="Array Prototype Every">
<h2>Array.fill()</h2>
<p>In this example, there is one array (foods).</p>
<p>In the change function, we are returning the output of foods.fill('kiwi', 2,5).</p>
<h3>array.fill() fills in the array and takes three parameters: the new element that will 'fill in' the old, the starting index, the ending index(this one will not be changed)</h3>
<p>In the example, 'kiwi' will be the new string element that will replace the other elements starting with the 2nd index until the 5th index (the 2nd, 3rd, and 4th, indexes will become 'kiwi') as seen in the console.</p>
<p>The result is:</p>
<p>['apple', 'orange', 'kiwi', 'kiwi', 'kiwi', 'lemon', 'mango', 'pear']</p>
<img src="images/Array Prototypes/arr.fill Example.png" alt="Array Prototype Fill">
<h2>Array.filter()</h2>
<p>In this example, there is one array (fruits).</p>
<p>The variable of favorites is being assigned the value of fruits.filter and then invoking a function of fruits that searches for any element in the array of fruits with a character length less than 5 characters.</p>
<p>The results are logged in the console as ['lime', 'pear']</p>
<h3>array.filter searchs through the elements of an array and for elements that meet a certain condition and returns a new array with all of the elements that passed the condition set inside the callback function.</h3>
<img src="images/Array Prototypes/arr.filter Example.png" alt="Array Prototype Filter">
<p>Here is another example of the array.filter() prototype in action.</p>
<p>In this example, any pet with the age of 10 will be returned in the new array.</p>
<p>An empty array is being returned because the function condition has not been met by any of the value of the object inside the array of pets.</p>
<img src="images/Array Prototypes/arr.filter Example copy.png" alt="">

