> select * from customers where _id = 'khannedy'
```
db.customers.find({
    _id: {
        $eq: "khannedy"
    }
});
```
> select * from products where price > 1000
```
db.products.find({
    price: {
        $gt: 1000
    }
});
```
> select * from products where category in ('handphone','laptop') > and price > 5000000
```
db.products.find({
    category: {
        $in: ["handphone", "laptop"]
    },
    price: {
        $gt: 5000000
    }
});
```
