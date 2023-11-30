# JavaScript

an array is a way to make a list or group of items
example:
let array = [snow,sand,dirt]

access methods in array
array.snow
array[1]

insert into an array
array.push('sky')
now array will say [snow,sand,dirt,sky]



an object will hold its data using {}
let animals = {
    cat: 'nib',
    dog: 'lou'
}

access an object
obj.cat
obj['cat']

change object
obj.cat = ['bill']



a function is a set of instructions
function hello() {
    console.log('Hello')
}


let catArr = [
    {
        name:bill,
        Weight: 10
    },
    {
        name: phill,
        weight: 11,
    }
]

access array items
console.log(catArr[i])
console.log(catArr.length)

for(let i = 0; i < catArr.length)

animals.foreach(lamdaFunction =>)

fire a function automaticly. functions for interval dont nee their () because setInterval is it's own function

setInterval(function, 1)

grab element by its class. needs a heros.forEach.(hero) if changing multiple heros
let test = document.getElementById(the id)

now we select the class inside test
let done = test.querrySelector('.class')

Next we have to draw these changes to the page
test.innerText = ${hero.name} | ${hero.health} | 

make objects move with html
marquee behavior = "alternate" direction= "left"

setTimeout calls a function once after a delay
setTimeout(animal => {
    function or code you need ran
}, 500)

save a score to local storage
let highScore = localStorage.getItem() pulls things out of local storage
localStorage.setItem('your highScore', highscore) sets something into local storage

if pull from local storage isnt a number and is stuck as a string then us
let highScore = parsInt(localStorage.getItem()) pulls things out of local storage
localStorage.setItem('your highScore', highscore) sets something into local storage

