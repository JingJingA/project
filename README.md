
/*取出 books 中 title 的值。*/const books = [
  {
    title: 'react', year: '2016',
  }
  {
    title: 'redux', year: '2017',
  }
];

----------------
const fun1 = (arr) => {
  var keys = [];
  for(var x in arr){
    keys.push(x);
  }
  return keys;
}

fun1(books) 输出 ["0","1"];

-----------------
const fun2 = (arr, year) => {
  var values = [];
  for(var y in arr){
    values.push(arr[y].title);
  }
  return values;
}

fun2(books, 2016) 输出 ["react"]

-----------------函数式编程（filter函数：过滤）
const getTitle (year books) => {
  const selected = filter(bk => bk.year == year, books);
  return map(bo => bo.title, selected);
}

getTitle(2017, books) 输出 ["redux"];




