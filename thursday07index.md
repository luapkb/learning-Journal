# Javacript notes

below are my notes in htmml

```


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>

    <h2>reading</h2> 
    <p> pages 1-24 ; 74-78 ; 88-94 </p>
    
    <h1>
        What is Javascript and how is it used
    </h1>
    <p> Javascript is a simple program that aids in makingweb pages more interactive.  It can be used to animate or provide comstomised input and output for a more useful exchange of information.  With Javascript a developer can offer an expanded veiw of a photo, provide the appropriate number of forms, preform calculaton. Javascript can specify that a script should run when an event occours such as cliking a link, pushing a buton hovering over and object on a page or simply after a time interval has elapsed.  
    </p>
    
<h2>writing a script</h2>
    <p>whe starting to wright a script its important to:</p>
        <ol>
            <li>define the goal of the srcipt 
                <p>start with the big pictuer. An example of a clear goal is, to provide the proper number of forms so that each person in a multible person booking can have an their card </p>
            </li>
            <li>designg the script 
                <p>this is often done by spliting the goal into smaller series of tasks.  it can ble recomended to do this by a flowchar for a visual reprisentiation of what needs to be done.  first you might want to know if they wanted vip or general addmition.  second you would want to know how many people in the party</p>
            </li>
            <li>actualy write the code 
                <p>javescript is a uniqe programing lanquage. the code for vip/general admition might look like this:
                    ''' 
                    function showOrder() {
                        var order = prompt('what would you like to order');
                        var item, quantity;
                        var items = '';
                    
                        while (order !== 'vip' && order !== 'general') {
                            order = prompt('please enter vip or general');
                        }
                        //ask quantity
                        quantity = prompt('how many would you like');
                        quantity = Number(quantity);
                    
                        //validate quantity
                        while (isNaN(quantity)) {
                            quantity = prompt('please enter a numaric value..');
                            quantity = Number(quantity);
                        }
                    
                        if (order === 'vip') {
                            item = '<this would be the filepath of the form>';
                        } else if (order === 'general') {
                            item = '<the file path of the form>'
                            // item = '<img src="images/house.png">';
                    
                            for (var i = 0; i < quantity; i++) {
                                items = items + item;
                            }
                            return items;
                        }
                    
                    '''


                </p>
            </li>

        </ol>




</html>
```
