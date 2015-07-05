###编写一个循环，将整数数组中相邻元素置换。Array(1,2,3,4,5) => Array(2,1,4,3,5)
```scala
object Test {
  def main(args: Array[String]) {
     val a = Array(1,2,3,4,5,6)
     for (i <- 0 until (a.length-1,2) if (i+1)%2!=0){
       a(i) = a(i)^a(i+1)
       a(i+1) = a(i)^a(i+1)
       a(i) = a(i)^a(i+1)
     }
    a.foreach(println)
  }
}
```
