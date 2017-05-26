# js-closure-this-index
通过闭包的运用改写tab选项卡 this的使用 及函数赋值

关注点：
1  aLi[i].onclick=showouter();相当赋值操作，就是不点击，把showouter()这个函数执行的结果赋值给了ali[li]，所以即便不点击 也会执行showouter()这个函数；
2  aLi[i].onclick=function(){
    //do sth
  }
  相当于让function这个工人A做某事  A又
  让B做某事
  
  aLi[i].onclick=showouter()//相当于直接让某个工作做某事。
  
 3 理解this不同位置所代表的含义。 
 aLi[i].onclick=showouter(this);//此处的this是在window内调用的 代表window。详细见代码，总的原则，谁调用，this就指谁。
 
