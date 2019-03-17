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
<p>The variable of favorites is being assigned the value of fruits.filter() and then invoking a function of fruits that searches for any element in the array of fruits with a character length less than 5 characters.</p>
<p>The results are logged in the console as ['lime', 'pear']</p>
<h3>array.filter searchs through the elements of an array for elements that meet a certain condition and returns a new array with all of the elements that passed the condition set inside the callback function.</h3>
<img src="images/Array Prototypes/arr.filter Example.png" alt="Array Prototype Filter">
<p>Here is another example of the array.filter() prototype in action.</p>
<p>In this example, any pet with the age of 10 will be returned in the new array.</p>
<p>An empty array is being returned because the function condition has not been met by any of the values of the object key age inside the array of pets.</p>
<img src="images/Array Prototypes/arr.filter Example copy.png" alt="">
<h2>Array.find()</h2>
<h3>Array.find() is very similar to array.filter() except it finds the first element that meets the condition and then returns the value of that element. Whereas array.filter() returns ALL of the elements that meet the condition and puts them in a new array.</h3>
<p>In this example, there is one array (fruits).</p>
<p>The function is asking it to look for the first element that is not 'apple'.</p>
<p>Thus, the console returns 'orange', the next element in the array that is not 'apple'.</p>
<img src="images/Array Prototypes/arr.find Example.png" alt="Array Prototype Find">
<h3>Array.find() Execution Table</h3>
<p>This table is based off a different example, but it shows the sequence of how array.find() is executed.</p>
<img src="images/Array Prototypes/arr.filter Example Table.png" alt="Array Prototype Find Table">
<h2>Array.forEach()</h2>
<p>In this example, there is one array (fruits).</p>
<p>The function is returning each element.</p>
<h3>array.forEach() executes a provided function once for each element in the array.</h3>
<h3>This prototype takes a callback function, index, array, and thisArg.</h3>
<img src="images/Array Prototypes/arr.forEach Example.png" alt="Array Prototype forEach">
<h3>Array.forEach() Execution Table</h3>
<p>This table is for a different example where the function is adding 1 to each element.</p>
<p>The output is below the table.</p>
<img src="images/Array Prototypes/arr.forEach Example Table.png" alt="Array Prototype forEach Table">
<h2>Array.includes()</h2>
<h3>array.includes() checks to see if the parameter is included in the array.</h3>
<h3>It returns a value of true or false.</h3>
<p>In this example, there is one array (fruits).</p>
<p>The function checks to see if 'berries' is an element in the array and returns true.</p>
<img src="images/Array Prototypes/arr.includes Example.png" alt="Array Prototype Includes">
<p>Here is the same array, however this time the function checks to see if 'watermelon' is the value of an element in the array.</p>
<p>It returns false.</p>
<img src="images/Array Prototypes/arr.includes Example 2.png" alt="Array Prototype Includes">
<h2>Array.indexOf()</h2>
<h3>array.indexOf() checks for the index of the passed in element. If the element is not in the array, it returns -1.</h3>
<p>In this example, there is one array (fruits).</p>
<p>The function checks for the index of 'lime' and returns 4 since 'lime' is in the 4th index of the array.</p>
<img src="images/Array Prototypes/arr.indexOf Example 2.png" alt="Array Prototype IndexOf">
<p>In this second example, using the same array, the function checks for 'watermelon'.</p>
<p>'watermelon' is not in the array so the console logs -1.</p>
<img src="images/Array Prototypes/arr.indexOf Example.png" alt="Array Prototype IndexOf">
<h2>Array.join()</h2>
<h3>array.join creates and returns a new string of all the elements via concatenation. By default, it returns each element seperated by a comma.</h3>
<p>In this example, there is one array (fruits).</p>
<p>The function joins together all of the elements. The seperator, by defualt, seperates them by commas.</p>
<img src="images/Array Prototypes/arr.join Example.png" alt="Array Prototype Join">
<h2>Array.map()</h2>
<h3>array.map creates a new array with the results of the function having been called on each element. It takes the parameters of (item, index, array)</h3>
<p>In this example, there is one array (evenNumbers).</p>
<p>The function is mapping over each element and adding one to the element's value. Those new numbers are returned and logged in the console.</p>
<p>[3, 5, 7, 9, 11]</p>
<img src="images/Array Prototypes/arr.map Example.png" alt="Array Prototype Map">
<p>This example uses the same array, but logs each number as the function maps over each element.</p>
<img src="images/Array Prototypes/arr.map Example 2.png" alt="Array Prototype Map">
<p>This final example contains an if statement.</p>
<p>If the number is 6, do nothing. Else add 1 to the number.</p>
<p>Looking at the console, you'll notice it returns undefined for the 2nd index where 6 used to be. That is because array.map must return something and if the return value has not been defined, then it returns undefined as a placeholder.</p>
<img src="images/Array Prototypes/arr.map Must Return Example.png" alt="Array Prototype Map">
<h2>Array.pop()</h2>
<h3>array.pop() removes the last element from the array and returns that element.</h3>
<p>In this example, there is one array (foods).</p>
<p>The function removes 'pear', the last element, and logs it in the console.</p>
<img src="images/Array Prototypes/arr.pop Example.png" alt="Array Prototype Pop">
<h2>Array.push()</h2>
<h3>array.push() pushes in new elements into the array and returns the new length of the array.</h3>
<p>In this example, there is one array (foods).</p>
<p>The function pushes in 'watermelon' and returns 9, the length of the new array.</p>
<img src="images/Array Prototypes/arr.push Example.png" alt="Array Prototype Push">
<h2>Array.reduce()</h2>
<h3>array.reduce() performs the reducer function on each element in the array and returns a single output. It has a callback function and takes the parameters (accumulator, currentValue, index, array).</h3>
<p>In this example, there is one array (fruits).</p>
<p></p>
<p></p>
<img src="" alt="Array Prototype Reduce">
<h2>Array.reverse()</h2>
<h3>array.reverse reverses the order of the array. The first element becomes the last.</h3>
<p>In this example, there is one array (foods).</p>
<p>The function reverses the order of the array and logs it in the console.</p>
<img src="images/Array Prototypes/arr.reverse Example.png" alt="Array Prototype Reverse">
<h2>Array.Shift()</h2>
<h3>array.shift() removes the first element of the array and returns that element.</h3>
<p>In this example, there is one array (foods).</p>
<p>The function removes the first element 'apple' and logs it in the console.</p>
<img src="images/Array Prototypes/arr.shift Example.png" alt="Array Prototype Shift">
<h2>Array.slice()</h2>
<h3>array.slice() returns a summarized version of the original array. It takes the parameters (begin, end). End is not inclusive.</h3>
<p>In this example, there is one array (fruits).</p>
<p>The function executes and returns the array contents from index 2 onward. (There is no end value as a parameter)</p>
<img src="images/Array Prototypes/arr.slice Example.png" alt="Array Prototype Slice">
<h2>Array.sort()</h2>
<h3>array.sort() sorts the array and returns the sorted version.</h3>
<p>In this example, there is one array (fruits).</p>
<p>The function sorts the array alphabetically and returns the modified version.</p>
<img src="images/Array Prototypes/arr.sort Example.png" alt="Array Prototype Sort">
<h2>Array.splice()</h2>
<h3>array.splice() changes the contents of the array by adding/replacing/removing existing elements. It takes the parameters (start, deleteCount, and item 1, item2...)</h3>
<p>In this example, there is one array (foods).</p>
<p>The function splices out the first two elements and returns the rest, starting at index 2.</p>
<img src="images/Array Prototypes/arr.splice Example.png" alt="Array Prototype Splice">
<h2>Array.unshift()</h2>
<h3>array.unshift() adds elements to the beginning of the array and returns the length of the new array. It takes the parameters (element 1....elementN).</h3>
<p>In this example, there is one array (foods).</p>
<p>Three new elements (2, 'watermelon', and 'peach') are added to the array, bringing the index count up to 11, which is logged in the console.</p>
<img src="images/Array Prototypes/arr.unshift Example.png" alt="Array Prototype Unshift ">

