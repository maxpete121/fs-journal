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