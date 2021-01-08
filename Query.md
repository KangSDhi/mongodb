> select * from customers where _id = 'khannedy'
```
db.customers.find({
    _id: "khannedy"
});
```

> select * from customers where name = 'Eko Kurniawan Khannedy'
```
db.customers.find({
    name: "Eko Kurniawan Khannedy"
});
```
> select * from customers where _id = 'khannedy' and name = 'Eko Kurniawan Khannedy'

```
db.customers.find({
    _id: "khannedy",
    name: "Eko Kurniawan Khannedy"
});
```

> Embedded Document

> select * from orders where items.product_id = 1
```
db.orders.find({
    "items.product_id": 1
});
```
