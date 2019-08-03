# DELETE Endpoints Functionality Study

<br>

## What is DELETE Endpoints Functionality Study?
The "DELETE Endpoints Functionality Study" demonstrates the basic functionalities of a DELETE request wherein the client removes an item from a list and any subsequent GET request will show the item removed.

<br>

In an express application, to handle a DELEET request, you call the app object (note the use of cond app = require('express') ) with the DELETE method. The DELETE method is pretty straight forward.  In the route handler, you need to provide the route AND the id of the item that you want to delete.  Then, when you request for the item to be deleted (i.e. req.params.id), you call the model and method (i.e. List.delete).


```JavaScript

                  app.delete('/list/:id', (req, res) => {                                
                    List.delete(req.params.id);                                           
                    console.log(`Deleted list item \`${req.params.id}\``);               
                    res.status(204).end();                                                        
                  });

```

<br>

## Does DELETE Endpoints Functionality Study feature commentary?
Yes! The DELETE Endpoints Functionality Study features commentary in the server.js file to show the structural context and implementation of POST endpoint functionality.  In addition, I also provide a Process text file that gives a good outline of the implementation process. 

<br>

## What are the key features of DELETE Endpoints Functionality Study?
Since this study is ongoing, basic functionalities are covered first and more advanced features are added or will be added in the future.  I divided this particular study into different branches covering different aspects of basic node servers, which I list below:


| **Features:**                            | **Feature Notes:**                             |
| ---------------------------------------- | ----------------------------------------------|
| DELETE request to localhost:8080/shopping-list/:id | This DELETE request will remove an item (and another GET request show it is gone) |


<br>

## Screenshots
![delete1](https://user-images.githubusercontent.com/37447586/62405290-9b5bb300-b550-11e9-941e-9e6e442c7145.png)
![delete2](https://user-images.githubusercontent.com/37447586/62405291-9b5bb300-b550-11e9-905a-e8b0fb5b242f.png)
![delete3](https://user-images.githubusercontent.com/37447586/62405292-9b5bb300-b550-11e9-8d5a-9eadd8d6957c.png)
