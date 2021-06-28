
# JSON

JSON stands for JavaScript Object Notation. JSON is an open standard file format and data interchange format that uses human-readable text to store and transmit data objects consisting of attribute–value pairs and arrays. 

## Running JSON

Use any of Your Favourite Browsers inspect it and then run it or any JavaScript Editor. Recommended Using 
[Chrome](https://www.google.com/intl/en_in/chrome/)

```bash
Ctrl+Shift+I
```

## Implementation

```
myJson=`{
    "name":"Aman",
    "score":"100",
    "isAdmin":true,
    "License":null,
    "shopItems":["Foods","Grocery","Beverages"],
    "myObj":{
        "name":"Vivek",
        "Grade":"A++",
        "Friends":["harshit","katiyar","Kartikey",{"no":"Vihaan"}]
    }
}`

parsed=JSON.parsed(myJson)
```

## Results

```parsed=JSON.parsed(myJson)  
parsed.name  --> Aman
parsed.License  --> null
parsed.shopItmes  --> ["Foods","Grocery","Beverages"]
parsed.shopItmes.length  --> 3
parsed.shopItmes[2]  --> Beverages
parsed.myObj  --> {
    "name":"Vivek",
    "Grade":"A++",
    "Friends":["harshit","katiyar","Kartikey",{"no":"aman"}]
}
parsed.myObj.Grade  --> A++
parsed.myObj.Friends.length  --> 4
parsed.myObj.Friends[2]  --> Kartikey
parsed.myObj.Friends[3].no.length  --> 1
parsed.myObj.Friends[3].no  --> Vihaan
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[2018eeb1139]()