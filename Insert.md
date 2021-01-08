> Insert Document Customers
```
db.customers.insertOne({
    _id: "khannedy",
    name: "Eko Kurniawan Khannedy"
});
```

> Insert Document Products
```
db.products.insertMany([
    {
        _id: 1,
        name: "Indomie Ayam Bawang",
        price: new NumberLong(2000)
    },
    {
        _id: 2,
        name: "Mie Sedap",
        price: new NumberLong(2000)
    }
]);
```
```
db.products.insertMany([
    {
        _id: 3,
        name: "Pop Mie Rasa Bakso",
        price: new NumberLong(2500),
        category: "food"
    },
    {
        _id: 4,
        name: "Samsung Galaxy S9+",
        price: new NumberLong(10000000),
        category: "handphone"
    },
    {
        _id: 5,
        name: "Acer Precator XXI",
        price: new NumberLong(25000000),
        category: "laptop"
    }
]);
```
```
db.products.insertMany([
    {
        _id: 6,
        name: "Logitech M235 Wireless Mouse",
        price: new NumberLong(175000),
        category: "laptop",
        tags: [
            "logitech", "mouse", "accessories"
        ]
    },
    {
        _id: 7,
        name: "Havit Cooler Pad Gaming 5Fan Blue led F2082",
        price: new NumberLong(200000),
        category: "laptop",
        tags: [
            "cooler", "laptop", "accessories", "fan"
        ]
    },
    {
        _id: 8,
        name: "Samsung LC24F390FHEXXD Curved Monitor ",
        price: new NumberLong(1750000),
        category: "computer",
        tags: [
            "samsung", "monitor", "computer"
        ]
    }
]);
```

> Insert Document Orders
```
db.orders.insertOne({
    _id: new ObjectId(),
    total: new NumberLong(8000),
    items: [
        {
            product_id: 1,
            price: new NumberLong(2000),
            quantity: new NumberInt(2)
        },
        {
            product_id: 2,
            price: new NumberLong(2000),
            quantity: new NumberInt(2)
        }
    ]
})
```
