# Node


The model still acts as instructions for the data it just does'nt store anything.

extend is a way to have another controller do exactly what another one does, but it can extent onto its functionality

if making an extended controller you need to make a super call after the constructor

export class CatsController extends BaseController{
    constructor(){
        console.log('loaded')
        super('api/cats')
        this.router //this lets you add the requests for the data you need
        .get('',this.getCat)
        .get('/test',this.test)
        .get('/:color', this.getCatColor)
    }

    test(request, response, next){ //these parameters will always come in this order
    response.send('<h1>Returns html tag</h1>') 
    }

    getCat(request, response, next){
        response.send('cats') // returns cats
    }

    getCatColor(request,response, next){
        if(request.params.color == 'orange'){
            response.send('cats orange')
        }else{
            throw new Error('Color not valid')
        }catch(error){
            next(error)// if its not orange this will send the data request to the next controller
        }
    }
}

console.logs will show up in your vscode console

IN SERVICE
const fakeDB ={
    cats =
    {name: 'Jimmy', color: 'orange', emoji: '🐈'}
}

getCats(){

}

POST

createCat(request, response, next){
    const payload = request.body
}




data model
export const CarSchema = new Schema({
    make:{type: String, maxLength: 25, required: true}
    model:{type: String, maxLength: 50, required: true}
    year:{type: Number, min: 1920, max: 2024, required: true}
    price:{type: Number, min: 0, required: true}
    description:{type: String, max: 1000},
    imgUrl:{type: String, maxLength: 500, required: true}
    engineType:{type: String, required: True, default: 'unknown', enum: ['two-cylinder', 'unknown']}
})

DBContext
Cars = mongoose.model('Cars', CarSchema)

class CarController{
    makeCar(){
    const carDAta = request.body
    const car = await carService.makeCar(carData)
    response.send(car)
    }
}

async getCar(request, response, next){
    const car = await carService.getCar()
    response.send(car)
}

async removeCar(request, response, next){
    const carRemove = await carService.removeCar(carId)
}


class CarService{
    makeCar(carData){
        const car = await dbContext.Cars.create(carData)
        return car
    }
}

async getCar(){
    const cars = await dbContext.Cars.Find()
}

async removeCar(carId){
    const carRemove = await dbContext.Cars.findById(carId)
    if(!carRemove){
        throw new Error('Cant find car at ${carId}')
    }
    await carRemove.remove()
    return `${carRemove.make}, ${carRemove.model} was removed`
}


ToJson: virtual
.populate calls to the virtual and tells it to fill with the exhibits
final step to attaching two data sets together

HOOK UP AUTH 0
put domain in the env domain section
along with client id
and audience

get auth token

open token, open preview, copy token
under auth tab in spaceman paste token into bearer token

when creating middleware
.use(Auth0Provider.getAuthorizedUserInfo)

in middleware
const userInfo = request.userInfo