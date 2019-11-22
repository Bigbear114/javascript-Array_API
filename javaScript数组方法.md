# **JavaScript 数组方法**
**1，Array.from() 方法从一个类似数组或可迭代对象创建一个新的，浅拷贝的数组实例。**
>**Array.from() 可以通过以下方式来创建数组对象：**  
. 伪数组对象（拥有一个 length 属性和若干索引属性的任意对象）  
. 可迭代对象（可以获取对象中的元素,如 Map和 Set 等）  
>>**`从String生成数组`**  
>>Array.from('array') //output：['a','r','r','a','y',]  
>>**`从Set生成数组(可用于数组去重)`**  
>>let set = new  Set(['app','ban','app','appear'])  
>>Array.from(set) // output: ['app','ban','appear']  
>>**`从Map生成数组`**  
>>let map = new Map([[1,2],[2,3],[3,4]])  
>>Array.from(map) // output:[[1,2],[2,3],[3,4]]  
>>  
>>let mapper = new Map([['1','a'],['2','b']])  
>>Array.from(mapper.values())   //['a','b']
>>
>>let mapper = new Map([['1','a'],['2','b']])  
>>Array.from(mapper.keys())  //['1','2']
----
