# MVC
the controller just tells the servic what is happeneing. the service makes things happen

start in models and put the blueprint to your objects data
export class character{
    name
    role
    class
    damage



    constructor(setName, setRole, setHealth){
        console.log('me')
        this.name = setName
        this.role = setRole || 'normal' -->this will make it pick between setRole and normal. can add more guidlines 
        this.health = setHealth
    }
}



use the appState to store the items that will use the blueprint you made

people = [
    new person('name','role','100')
]
/** @type(people)*/ this will tell the select person that it is going to be a person so you can edit values
selectPerson = null
/**@type(people[]) this is how you set an arrays type




draw your data to the page using the controller
export class = theTestController{
    constructor(){
        this.drawStuff()
    }
    drawStuff(){
        
    }
    selectService(){
        testService.selectService
    }
}



you now need to import your controller to app.js
in class app
testclassToUse = new TestClassToUse()

observers will take place in the controller
appState.on('selectPerson', this.drawFunctionYouNeed)





the router looks at the website brouser url and loads a route
as the router changes routes it relaods any controllers and injects the view onto the html with the id router-view
set view to null to stop the router from loading things into your view




the service is where you put the actual function you want to run and what the function runs
class TestService{
    selectService(){
        test+ 2
    }
}
export const testService = new TestService



findIndex just returns its position while find returns the item it finds

splice remove an array  the.splice(startpoint, 1) number is how many items to remove



router

path:
constructor[]
view: ''


forms
use form handler
const formData = getFormData(form)

new constructor does not need multiple passthroughs
constructor(data){
    this.make = data.make
    this.model = data.model
    this.year = data.year
}

appState look
this will pull all the data at once from the new constructor

cars = [
    new Car({
        make:
        model:
    })
]


everything in a form will come out of it as a string
formData.yourvalue = parseInt(formData.yourvalue) this will change your string data into a value


event.preventDefault() this will stop a form from 
const form = event.target the target is the form itself this will grab the entire form
const formData = new FormData(put in html form element)

form.reset() this will reset the form and clear all data imputed upon pressing the submit button

name="" gives inputs a name to use to tell javascript where a forms info needs to go and what information is what.


can use the fancy confirm but need to use these extra steps
async and await will pause the function to let the user confirm
async function(card){
    let confirm await Pop.confirm("words in the alert promt")
    if(confirm){
        carsService.function(card)
    }
}


save and load to local storage
function(){
   saveState('cars', appState.cars)
}

loadCars(){
    let loadedCar = loadState('cars', [car])
    appState.cars = loadedCar
}


forms

createNewCase(){}
event.target will grab form
const form = event.target
this makes form take on the form in full
const formData = getFormData(form)
this lets formData get the data from the form we made just above
caseFileService.createCaseFile(formData)
this links this function to its other half in the service

in the service

createNewCase(formData){
    const newCaseFile = new CaseFile(formData)

    appState.casefiles.push(newCaseFile)
    this pushes the form file you made into your appState to become a new object
}


${this.locked} ? ${this.LockedCaseFiled} : ${this.unlockCaseFile}
this will look at the true false. if its true it will draw the first option. If false it will draw the second item given




