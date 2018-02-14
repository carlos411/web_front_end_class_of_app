# 4.1.9 物件\(Object\)

結構語法

![](/assets/object_basic1.png)

## 觀念

任何人、事、物都可以是物件\(Object\)，都有自己的屬性及動作。

以車子為例，車子本身就是一個物件，屬性有廠牌名稱、總量等；可以執行的動作有開車、停車。

## 範例：瞭解 dot syntax

瞭解物件結構，以及如何使用物件：

```js
var car = {
  brand_name: "toyota",
  weight: "500kg",
  doors: 4,
  drive: function(){
    alert("drive");
  },
  stop: function(){
    alert("stop");
  }  
};

car.drive();
car.stop();
alert(car.brand_name);
```

## 練習

執行上述範例程式，並瞭解物件結構，以及執行的語法

