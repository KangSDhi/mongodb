> select * from products where (tags = "samsung" and tags = "monitor")
```
db.products.find({
    tags: {
        $all: ["samsung", "monitor"]
    }
});
```

> select * from products where tags in ("samsung",  "logitect")
```
db.products.find({
    tags: {
        $elemMatch: {
            $in: ["samsung", "logitech"]
        }
    }
});
```

> select * from products where size(tags) = 3
```
db.products.find({
    tags: {
        $size: 3
    }
});
```
