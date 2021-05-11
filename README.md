# Week 1
 ### Here's what I learned so far:

 * ## HTML
    * DIVs to group items together
    * IDs to identify one item
    * Classes to identify items belong to the same class
    
 * ## CSS
    * ### Flex-box
      * I learned how to easily align boxes using ***display:flex***. Use ***justify-content*** to put it in a column or row and ***align-items*** to put boxes in the center.
    * ### Properties
      * I learned more properties like ***border***, ***font-family***, ***float***, ***margin***, ***padding***, ***border-radius***
    * ### Hover animations 
* ## Bash
    * Create directories using ***mkdir***
    * Remove directories using ***rmdir -ef***
    * Creat files ***touch***
    * Remove files ***rm***
    * Move or rename files ***mv***
    * List file ***ls***
    * List all files ***ls -a***
    * Copy files ***cp***
    * Change directory ***cd***



# Week2

## Early week

We did instabox group assignment to advance our flexbox skills. 
- 1. We identified page's structure
- 2. One person worked on upper part
- 3. I worked on stories
- 4. In the end we've got pretty good result

![instabox](https://i.imgur.com/tACIJY0.png)
#

Later we created out personal webpage.
I learned how to make a video as a background.


```
HTML

  <video autoplay muted loop id="vid"> 
  <source src="https://i.imgur.com/37MESxa.mp4" type="video/mp4"/>
  </video>
```

```
CSS

  position: fixed;
  right: 0;
  bottom: 0;
  min-width: 100%;
  min-height: 100%;
```
Final result:
![](https://media2.giphy.com/media/EbwvwkfPvlKENhe6sW/giphy.gif)

## Mid-week

We started learning grid.
First, we need to identify rows, columns and their sizes.

##### *Example:*
```grid-template-columns: 25% 25% 25% 25% ``` or ``` grid-template-column: repeat (4, 25%)``` - there will be 4 coulmns with equal width.
```grid-template-rows: 50% 50%``` - both rows will have equal height.

Then we need to assign each cell to one group.

##### *Example:*

```
#cell-1{
  grid-column: 2;
  grid-row: 1;
}
```

If we want to merge one row than we have to put to numbers and a slash between them. The first number shows at the beginning of what column the row starts, and the second one at the beginning of what column does it end.

##### *Example:*

```
#cell-1{
  grid-column: 2;
  grid-row: 1/3;
}
```

We also can use areas:
```
CSS

#cell-1{
  grid-template-column: 25% 70% 5%;
  grid-template-row: 25% 75%;
  grid-template-areas: 
  " a b c"
  "d . c"
}

#a{
  grid-area: a;
}

#b{
  grid-area: b;
}

#c{
  grid-area: c;
}

#d{
  grid-area: d;
}
```
###### P.S A dot means empty space.

## Late week

We had a Twitter post assignment.

The code can be find [here](https://repl.it/@NSKvak/twitter-gridder-1#index.html).

Final version:
![](https://i.imgur.com/ji8pp67.png)

Then we learned about wireframes. 
I did one for Monster website.
The code for monster website can be find [here](https://repl.it/@NSKvak/copy-ocelot#index.html).

![](https://i.imgur.com/jssIMv3.png)





# Week 3

### Collaborating on VSC

I learned how to fork, clone, push and pull codes using terminal.
* First we need to fork the code if we haven't been granted an access. 
* Then we need to clone it by copying the ink `cmd+l, cmd+c`, then in terminal type `git clone "link"` end hit enter.
* After changing the code, we go to terminal to add modifictations `git add index.html`
* Then commit `gti commit -m "Adds title"`
* And push `git push`
* To pull changes others made we use `git pull`

### Shortcuts
* `cmd+left/right arrow` - moves to the begininng/end of line
* `opt+left/right arrow` - moves by words
* `cmd+up/down arrow` - moves to the beginning/end of code
* `opt+up/down arrow` - moves current line to the line above/bellow
* `cmd+\` - split view
* `cmd+1,2,3` - move between split views
* `control+space` - opens terminal
* `cmd+control+f` - full screen
* `com+d` - select current word, several clicks select the same words
* `option+shift+down arrow` - copies the line
* `f2` - changes all the same names
* `cmd+shift+k` - deletes the line
* `cmd+shift+p` - find everything

### Java Script
* Make variables: `let x = 8;`
* String - actual words/letters: `x = '2';`
* Numbers: `x = 2;`
* Booleans - binary statemnasts: true/false
* Functions: `function varibleName (x){ *code* 
}`  
* Print something: `console.log(x);`
* Java script reads lines one-by-one, so if the variable changed before it's printed, it will show the original one.
* in terminal use `jest --watch-all` to test the code with main.test.js



# Week 4

## Tips
* `codemon name_of_file` - to see if it's working on terminal and it will update automatically
* `code name_of_file` - to check if the code is working on terminal

## Strings
* `name.length` - the length of a string
* space counts as a character
* `name.toUpperCase()` - change all letters capital
* `(3).toString` - changes numbers to strings
* `(301.45346876).toFixed(2)` - will leave only 2 numbers after point
* index - the order number of a character in a string. It's zero-based
  * `result = 'Hello'[0]` result will return H
  * `number.slice(-4)` - will return last 4 digits
* name.indexOf('a) - will find the index number of that letter in a string.

## Booleans
* === is not ==: === means **exactly the same** while == means **somewhat the same**.
* !== means **not equal**
* && means logical **and** operator
* || means **or**

## return vs console.log
***console.log*** shows it only for developer when ***return*** actually returns something for everyone.

## IF statements
* `if (grade < 60){
  return 'F'
} else if (grase < 70>){
  return 'You got a C'
}` - if-else statements

## let vs const
You can change **let** later but can't change **const**. Both of them cannot be reassigned, but we can change const to let in an original code.

* Property is a variable that's stored as part of another
* A characteristic or attribute of that variable
* For strings, the main one is length

* A method is a special kind of property that's a FUNCTION




# Week 5

* ## Switch syntax:
``` 
switch (num){
    case 1:
      return "Sunday"
    default:
      return "Wrong"
} 
```

* ## Node/ input syntax:
```
const getInput = require("./get-input.js");
const name =  getInput();
console.log("Hi, " + name);
```
` node filename.js Nastya` will show Hi, Nastya in terminal.
* #### To use getInput we should first store a variable. If there are **two** argeuments we should write getInput(0), getInput(1) for the first two.

* #### To run prettier we should turn auto-save off, check format on save, and when changing codes, click cmd+s, and run format on prettier.

* #### To use code from another file we can copy that file using terminal. *For example*: `cp ../fizzy/fizzy.js fizzy-backend.js` and then on fizzy-backend.js delete curly brackets. *Example:* `module.exports = {fizzy}` change to `module.exports = fizzy` and on fizzy.js write 
```
const fizzy = require("./fizzy-backend.js");

const number = getInput();
const answer = fizzy(number);
console.log(answer);
```
Don't forget to save.

* ### To return input there is a code: 
```
function getInput() {
  return process.argv[2];
}

module.exports = getInput;
```
#### Then we can use `const name = getInput()`
#### If there are several arguments use `getInput(1) and getInput(2)` depending on counting base.

* `str.inscludes('')` or `str.endsWith('')` - to check if a string ends with a particular characters




# Week 6

## New Syntax
- have *${var}* will run the variable inside the quote, thus, conjugation is not needed for a string and variable.
```
const myName = 'Nastya'
const hello = 'hello ${myName}'
```  

* `console.log('We\'re in New York')` - if we use single quotes we should use \ for single quote that is part of a string

* empty string is considered false:
```
const value = '';
if(value){
  console.log('asdf')
}
```
###### it will return nothing.

#### Truthy values:
* 'asdf'
* "asdf"
* 1, -2, 1.1
* true
#### Falsy values:
* ''
* ""
* 0
* false
* undefined


```
const e = 'asdf' === 'asdf'
console.log(e)
```
###### will return **true**


## Arrays methods
* Push adds a new element to the end of the array
`arr.push(5)`
* Pop removes the last element to the beginning of the array
`arr.pop()`
* Unshift adds an element to the beginning of the array
`arr.unshift()`
* Splice can remove and add elements from an array
`arr.splice(1,1)`
`arr. splice (1, 1, "Line", "Dot")`
* Shift removes the fisrt item
`arr.shift('Banana')`
* Slice splits one arrays into several. One argument says from where the new array stars, the second d=number says where it ends not including that number.
`arr.slice(1, 3)`
`arr.clice(2)`
* Concat is merging several lists into one
`const arrSum = arr1.concat(arr2, arr3)`
* Reverse arrays
`arr.reverse()`
* Join chahges arrays to string and chooses separators
`arr.join('*')`

## Loops
* To print all items from array we cn use this code:
```
for (const item of arr){
  console.log(item)
}
```

* For of loop/ for each loop
```
for (const letter of variable){
  console.log(letter)
}
```

* Reduce - take all the values in the array, produce a new single value based on all the values in the array
```
const nums = [1, 2, 3, 4];

let sum = 0;
for (const vause of nums){
  <!-- sum = sum + value;  -->
  sum +=value
}
console.log(sum)
<!-- for (let i = 0; i < nums.length; i++){
  const value = nums[i]
} -->
```
* Map - create a new array where we apply a transformation to each item of the array
```
const nums2 = [1, 2, 3];
let output = [];
for (const value of nums2){
  output.push(value*2)
}
console.log(output)
```
or
`nums2.map(n => n*2)`

* Filter - output in an array with equal to or fewwer elements as the input array
```
const nums3 = [1, 2, 3, 4, 5, 6, 7]

let output2 =[];
for (const value of nums3){
  if (value <=3){
    output2.push(value)
  }
}
```


# Week 7

```
If (char === “ “){
ShouldCapitaalized = true
} else {
ShouldCapitalized = false
}
```

Simplification:
`shouldCapiatalised = char === ‘ ‘`

If we need to change true to false and vice verse use simplification:
`ShouldCapitaalized = !ShouldCapitaalized`

* `continue` skips the iteration from the loop

## Array methods 
##### * .split
to make str an array 

#### * .join
join a list into a. str using a separator

#### * .reduce
take in array and gives an output

```
function sum2(num)
  const sum = array.reduce(
    (sum,num) => sum+num, 0
  )
  return sum
```

#### * .map
Takes in array, maps each value to another value (output is array)
```
function arrayDoubler (numArray){
  let output = []
  for (const num of numArray){
    output.push(num * 2)
  }
}
```
or 
```
function arrayDoubler2(numArray){
  const output = numArray.map(
    (num) => num*2
  )
  return output
}
```
no need "return"

#### * .filter
take in array, return an array with some values filtered output
```
function lessThan5(arr){
  let output = []
  for (const num of arr){
    if (num<5){
      ouput.push(num)
    }
  }
   return output
}
```
or
```
function lessThan5Two(arr){
  const output = arr.filter(
    (num) => num<5
  )
  return output
}
```

### Regex (regular expressions)
/a/.test ('abc') - abc contains a
true
/\s/.test ('abc ') - contains spaces
true


## Objects
Keys - unique values inside one object.
*For exp:*
*'123 Main Str': 94120*
*'450 12th Blvd: 94120*
*'320 Putnam Ave: 94120*
 *Real object example:*
 ```
 const addresses toZipCodes = {
  *'123 Main Str': 94120*,
  *'450 12th Blvd: 94120*,
  *'320 Putnam Ave: 94120*
 }
 ```
or 
```
const user = {
  firstName: 'Nastya',
  lastName: 'Kvak',
  email:'nkvak@fordham.edu',
  phone: '1293454324'
  friends:[Lily, Dari, Vlad]
}
```
### Getting properties

#### to print a value of a particular key, we should use 
`console.log(user.firstName)`
#### to print the list items in value
`console.log(user.friends[2])`

### Setting properties on the object
#### new keys with values
`user.shirtColor = 'blue'`

#### dot and bracket notations
`user.shirtColor = 'blue'`
same as 
`user['shirtColor'] = 'blue'` - needed when there are spaces. or 
```
const key = 'shirtColor; 
user[key]='blue'
```
### Objects in objects 
```
const nestedObject = {
  playlistName: 'my jams',
  songs:[
    {
      songName: 'Hey Ya!',
      songLength: 2
    }
  ]
}
```

## Mutation

The function can mutate objects and arrays
`delete object.lastName` - to delete object property



# Week 8

## Create repositories

* Go to repositories
* Create a new one
* Clone it
* Copy to create read.me


If you have something on your USERNAME.github.io repo already and want to save your work on a branch,
* Clone the repo, git clone ...
* Enter the repo, cd USERNAME.github.io
* Put your current work on a branch (named backup in this case), git checkout -b backup
* Push your branch to the Github, git push -u origin backup
* Go back to the master branch (this is sometimes called main instead of master), git checkout master
* Delete everything on that branch rm -rf * (Warning: dangerous command, make SURE you are in the correct folder before running this)
* Make a commit
* Push the changes

To quickly commit use -am instead of -m

## Connect JS to HTML and CSS
* `const bigTitle = document.querySelector('.big-title')` -  gives an object that returns part of HTML

* bigTItle.innerHTML = "<div>asdf</div" - will change attributes on HTML

* `bigTItle.style.fontSize = '100px'` - changes font size;

* `const bigTitles = document.querySelectorAll('.big-title')` - to get all things under the same class.

* assign color
```
const secondBigTitle = bigTitles[1]`;
secondBigTitle.style.backgroundColor = 'blue'
``` 

* changes image source
```
const image = document.quwtySelector ('img');
image.src = 'http://www.tioxic.com/wp-content/uploads/trex_4.jpg'
```
* first parameter is the event, second is function
```
function changeBackgroundToGreen(){
  consoe.log('change backeground to green')
  const body = document.querySelector('body');
  body.style.backgroundCOlor = 'green'
}

`button.addEventListener ('click', changeBackgroundToGreen)` 
```

* different params for addEventListener
```
element.addEventListener("mouseover", myFunction);
element.addEventListener("click", mySecondFunction);
element.addEventListener("mouseout", myThirdFunction);
```

### Anonymous functions
```
thing.addEventListener ('click', function (){
  actual function content
})
```
or
```
thing.addEventListener ('click', () => {
  actual function content
})
```

### Add Event Listeners in a loop

```
const purpleBox = document.querySelectorAll('.small-inner-box');

for (const box of purpleBoxes){
  box.addEventListener (click, function (event){
    const elementThatWasClicked = event.target;
    elementThatWasClicked.style.backgroundColor = 'green'
  })
}
```

### Elelment transitions
```
.transition-element{
  transition: all 3s linear
}
// * ease
// * linear
.invisible{
  opacity: 0;
}
```
```
const pinkSquare = document.querySelector(.transition-element);
pinkSquare.addEventListener('click', function(){
  pinkSquare.classList.add('invisible')
})
```
### Create element
```
const title = document.createElement('h1');
title.style.color = 'white';
title.style.fontFamily = 'Arial, sans-serif'
title.innerText = 'string of something'

container.appendChild(title)
```

* remove title
```
title.remove()
```
* firts child refers to the first thing we put in there
```
const tit;e2 = document.createElement (h3')
title2.innerText = "another string"
container.appendChild(title2)

container.firstChild
```




# Week 9

`element.lastElementChild` - return actual item, not a white space

### Functions expressions
```
const functionExxpression = function(){
  console.log('function expression')
}
```

### Arrow expressions
```
const arrowFunciton = () => {
  console.log('arrow function')
}
```

```
const add = (a,b)=>{
  return a+b
}
```

Both expressions are not hoisted, you can't call them before they are defined

### Random
`Math.random()`
```
function getRnadom (){
  const randomecimal = Math.random();
  const scaledRandom == randomDecimal *3
  return Math.floor(scaledRandom)
}
```
### Array sorting

const a = ['c', 'b']
a.sort();

<!-- This will sort it alphabeticallym which is wrong! -->
console.log = ['-2', '-1', '0', '1', '2']
b.sort()
console.log(b)

b.sort(a, b)=>{
  return a-b;

}

### Input, forms

```
<input type="text" placeholder="something" />
<form>
  <div>
    <input type="radio"  name = "radio-group-1"  value ="apple"/>
    <label>Apple</label>
  </div>
   <div>
    <input type="radio"  name = "radio-group-1" value="orange"/>
    <label>Orange</label>
  </div>

</form>
```
* name - group radio buttons so only one can be selected 
* value - to see which one was clicked because label is a separate thing from input
* label - to label different options, it's separate from input (usually the same as label)
* form - groups input together
* button goes under form
* placeholder - is what is inside the input box by default

```
const radios = document.querySelectorAll('[name="radio-graoup-on"]')
for (const of radios){
  if(radio.checked){
    console.log(radio.value)
  }
}
```
* instead of name we can also use type in querySelectorAll
* radio.checked - to see which one is checked
* radio.value - will return value

```
const textInput=document.querySelector('[type="text"]')
console.log(textInput.value)
```
returns text input





# Week 10
## Responsive website

```
@media screen and (max-width:300px){
  .item-1{
    border:2px solid green
  }
  .item-2{
    padding:20px
  }
}
```
`if(window.innerWidth=300px)`





# Week 11

* Delaying of execusion of the code
1500=1.5 secons
`setTimeout(helloWirld, 1500)`

* Repeating every 5 ms
`setInterval(helloWorld, 500)`

### Create sound

`const audio = new Audio('tick.mp3)` - gives us audio object
`audio.play()` - you can put it into a function to play the audio object

## Checkbox
```
<input type='checkbox'>
<label>Our checkbox</label>
```

const checkbox = document.querySelector('input')
`ckeckbox.checked` - to see if thebox is checked

## API
```
<!-- Make a request to url -->

const URL= "link.com"

<!-- Add event listener -->

button.adEventListener('click', ()=>{


  fetch(URL)

   <!-- process the raw response into object -->

    .then(function (rawResponse) {
      console.log('response success!')
      console.log('raw response', rawResponse)
      return rawResponse.json()
    })

    <!-- take the object and do whatewer you like -->

    .then(function (json){
      console.log('response object acquired')
      console.log('JSON', json)
    })
})
```
or 
```
const URL = 'link'

fetch(URL)
  .then((res) => res.json())
  .then((data)=>{
    console.log('success')
    console.log(data.message)
  })
```




# Week 12

## Asynch promise/callbacks

```
function promiseFunction (){
  return new Promise ((resolve) => {
      setTimeout(resolve, 1000);
});
)
}

promiseFunction()
  .then(() => {
    console.log ('hello world')
    return promiseFunction()
  }
  .then(() => {
    console.log ('second request completed')
    return promiseFunction()
  })
  .then(() => {
    console.log('third request completes)
  })
  ```

  ## With fetch
  ```
const img = document.querySelector('img')

  fetch(url)
    .then(rawResponse) => rawResponse.json())
    .then (dogImageObject) => {
      img.src= dogImageObject.message;
      return fetch(url)
    })
```


##

const NORAD = "123 534 6"
encodeURI(NORAD)




# Week 13

## jQuery
```
 <script
        src="https://code.jquery.com/jquery-3.6.0.min.js"
        integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4="
        crossorigin="anonymous">
  </script>
```

### Create new DOM element using jQuery
```
//Query select button element
const jQueryButton = $ ('button')
//Add event
jQueryButton.click(function () {
  const newItem = $('<div class="item">new item</div>')
  newItem.text('this is the new new text')
  const container = $('.container)
  container.append(newItem)
})
```

we can also combine code like this:
```
$('button').click(function(){
  const newItem = $(<div>new item</div>)
  $(container).append(newItem)
})
```

value = val
innerHTML = HTML

## Local storage 

window.localStorage.getItem()

window.localStorage.setItem()

```
const input = $('input')

const previousInputText = window.localStorage.getItem('inputText')
if(previpusInputText !== null){
  input.val(previousInputText)
}

input.change(function (){
  console.log(input.val)

  window.localStorage.setItem('inputText', input.val())
})
```
`window.localStorage.clear()` - to clear local storage

`JSON.stringify()` - to make it a string
`JSON.parse()` - to change it back from a string

## Loop using jQuery

```
const btns=$(',item)
for (const rawButton of btns){
  const button = $(rawbutton)
  button.click(function(){
    console.log(button.text())
  })
}
```# Term-1-Notes
