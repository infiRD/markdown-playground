#Scala cheat-sheet

- [Current Scala ScalaDoc][11]
- [Coursera/Scala progfun1 cheat-sheet][7]

##Zapis funkcii:

```Scala
x => x                            // anonymous identity function
def id(x: Any) = x                // identity function
          def g(v: Int) = v + 1
l.map(x => g(x))                  // rovnocenny zapis ako nizsie
l.map(g)                          // rovnocenny zapis ako x => g(x)
map.filter(e => e._2 > 'a')       // anonymous function with Tuple: select only characters with code larger than 'a'
map.filter{case (_,v) => v > 'a'} // anonymous function with 'unapply' to directly match Tuple2 - (k,v)
tweets.foreach(x => res += x)     // this is equavalent 
tweets.foreach(res += _)          // to this
```

 [11]: https://laverna.cc "Official Laverna site"
 [7]: https://github.com/Laverna/laverna "Laverna GitHub repo"

 








