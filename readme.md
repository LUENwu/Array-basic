# 数组测试题

## 1. 把数字变成星期

```
map()方法

let day = ['周日','周一','周二','周三','周四','周五','周六']
或
let day = {
  0: "周日",
  1: "周一",
  2: "周二",
  3: "周三",
  4: "周四",
  5: "周五",
  6: "周六",
};


let arr = [0, 1, 2, 2, 3, 3, 3, 4, 4, 4, 4, 6]

let arr2 = arr.map(item => return day[item])

console.log(arr2) 
//['周日', '周一', '周二', '周二', '周三', '周三', '周三', '周四', '周四', '周四', '周四', '周六']


reduce()方法

let day = ['周日','周一','周二','周三','周四','周五','周六']

let arr = [0, 1, 2, 2, 3, 3, 3, 4, 4, 4, 4, 6]

let arr2 = arr.reduce((result,item)=> return result.concat(day[item]),[])

```
如图 ![图](/image/屏幕截图%202022-01-07%20030339.jpg)
##  2. 找出所有大于 60 分的成绩
```
filter()方法

let scores = [95,91,59,55,42,82,72,85,67,66,55,91]

let scores2 = scores.filter(item => item > 60 ).sort().reverse()

console.log(scores2)//


reduce()方法

let scores = [95,91,59,55,42,82,72,85,67,66,55,91]

let scores2 = scores.reduce((result,item)=> result.concat(item>60?item:[]).sort(),[])

```
如图![](/image/屏幕截图%202022-01-07%20033415.jpg)

## 3. 算出所有奇数之和
```
let scores = [95,91,59,55,42,82,72,85,67,66,55,91]

let scores = [95,91,59,55,42,82,72,85,67,66,55,91]
let sum = scores.reduce((sum, n)=>{
 return n%2===1?sum+n:sum
},0)
console.log(sum)
```
如图   
![](/image/数组reduce.jpg)