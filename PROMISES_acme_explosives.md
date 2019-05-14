# Acme Explosives


## Requirements

You are going to be creating several JSON files that will be describing all of the explosive products that you sell. You need to use Promises to handle the order of the asynchronous operations needed to load the data.

### Product Categories

Choose at least two, but as many of you like, categories for your products. Give each one an integer unique id.

Here's an example.

##### categories.json

```js
{
    "categories": [
        {
            "id": "category0",
            "name": "Fireworks"
        },
        {
            "id": "category1",
            "name": "Demolition"
        }
    ]
}
```

### Product Types

Create a JSON file describing types **for each** category of your products. For each type, add a key/value pair that creates a relationship to the corresponding category. Create at least 3 types for each category.

##### types.json

```js
{
    "types": [
        {
            "id": "type0",
            "category": "category0",
            "name": "personal",
            "description": "Fireworks intended for recreational use during holiday celebrations"
        }
    ]
}
```

### Product Details

Create a JSON file describing each product you offer. Add a key/value pair that creates a relationship to the appropriate product type. Add at least 3 products for each type.

##### products.json

```js
{
    "products": [{
        "fairy_sparklers": {
            "id": "product0",
            "type": "type0",
            "name": "Fairy Sparklers",
            "description": "Multi-colored sparklers that are safe for any age."
        }
    }]
}
```


### Display
use Promises to read, first, from the `categories.json` to load that array of objects, then load `types.json`, then `products.json`.  Once you have all the data display each product as a bootstrap card - 4 to a row.  Each card should say the name, description, product name, type name, and category name for that product.


### Bonus
On page load a user should see a dropdown menu that gets populated with category names after the promise for categories.json loads.

When a user selects a category they should only see the products that belong to that category.
