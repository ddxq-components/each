each
==========

一个通用的迭代函数，它可以用来无缝迭代对象和数组。
数组和类似数组的对象通过一个长度属性（如一个函数的参数对象）来迭代数字索引，从0到length - 1。其他对象通过其属性名进行迭代。

----------

## 使用说明

### each(<array,object>, callback, context)


``` javascript
var each = require('each');
each([52, 97], function(index, value) {
  alert(index + ': ' + value);
});
```

``` javascript
var each = require('each');
var obj = {
  "flammable": "inflammable",
  "duh": "no duh"
};
each( obj, function(key, value) {
  alert(key + ": " + value);
});
```