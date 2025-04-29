# cs2030-lab-8--infinite-list-solved
**TO GET THIS SOLUTION VISIT:** [CS2030 LAB 8- Infinite List Solved](https://www.ankitcodinghub.com/product/cs2030-infinite-list-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114519&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS2030 LAB 8- Infinite List Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Problem Description

An infinite list InfiniteList is a generic list that can store elements of type T in order where duplicates are allowed. Unlike the previous lab, intermediate operations of InfiniteList should be lazily evaluated.

The Task

You are to design your own InfiniteList interface with the following requirements below. As InfiniteList is similar to Java’s Stream in Java, and so, you are not allowed to import packages from java.util.stream

Create the InfiniteList interface and the InfiniteListImpl implementation Define a get method for each operation

This task is divided into several levels. Read through all the levels to see how the different levels are related. You need to complete all levels.

Just remember to:

Level 2

Implement the following intermediate operations following the corresponding specifications of Java’s Stream API:

InfiniteList&lt;R&gt; map(Function&lt;T, R&gt; mapper)

InfiniteList&lt;T&gt; limit(int maxSize)

InfiniteList&lt;T&gt; filter(Predicate&lt;T&gt; predicate)

InfiniteList&lt;T&gt; takeWhile(Predicate&lt;T&gt; predicate)

As some of the methods could possibly produce no elements, you will need to redefine get to have a return type of Optional&lt;T&gt;.

jshell&gt; /open InfiniteListImpl.java jshell&gt; /open InfiniteList.java

jshell&gt; InfiniteList&lt;String&gt; ifl = InfiniteList.generate(() -&gt; “A”).map(x -&gt; x + 1) ifl ==&gt; InfiniteListImpl$2@28d25987

jshell&gt; IntStream.range(1, 5).forEach(x -&gt; System.out.println(ifl.get())) Optional[A1]

Optional[A1]

Optional[A1] Optional[A1]

jshell&gt; InfiniteList&lt;Integer&gt; ifl = InfiniteList.iterate(1, x -&gt; x + 1).filter(x -&gt; x % 2 == 0) ifl ==&gt; InfiniteListImpl$3@7cd62f43

jshell&gt; IntStream.range(1, 5).forEach(x -&gt; System.out.println(ifl.get())) Optional[2]

Optional[4]

Optional[6] Optional[8]

jshell&gt; InfiniteList&lt;Integer&gt; ifl = InfiniteList.iterate(1, x -&gt; x + 1).limit(2) ifl ==&gt; InfiniteListImpl$1@39c0f4a

jshell&gt; IntStream.range(1, 5).forEach(x -&gt; System.out.println(ifl.get())) Optional[1]

Optional[2]

Optional.empty Optional.empty

jshell&gt; InfiniteList&lt;Integer&gt; ifl = InfiniteList.iterate(1, x -&gt; x + 1).limit(2).filter(x -&gt; x % 2 == 0) ifl ==&gt; InfiniteListImpl$3@53b32d7

jshell&gt; IntStream.range(1, 5).forEach(x -&gt; System.out.println(ifl.get())) Optional[2]

Optional.empty

Optional.empty Optional.empty

jshell&gt; InfiniteList&lt;Integer&gt; ifl = InfiniteList.iterate(1, x -&gt; x + 1).takeWhile(x -&gt; x &lt; 3) ifl ==&gt; InfiniteListImpl$4@3abbfa04

jshell&gt; IntStream.range(1, 5).forEach(x -&gt; System.out.println(ifl.get())) Optional[1]

Optional[2]

Optional.empty

Optional.empty

Make a copy of your Java programs to the level directory by typing the Unix commands

$ jar cvf infinite2.jar *.java

$ mkdir infinite2

$ cp *.java infinite2

$ cp infinite2.jar infinite2

Verify your jar archive using

$ jar tf ~/infinite2/infinite2.jar

Level 3

Now implement the following terminal operations by following the corresponding specifications of Java’s Stream API:

long count()

void forEach(Consumer&lt;T&gt; action)

Optional&lt;T&gt; reduce(BiFunction&lt;T,T,T&gt; accumulator)

T reduce(T identity, BiFunction&lt;T,T,T&gt; accumulator) Object[] toArray()

You will also need to ensure that the get method can no longer be called from a client class.

jshell&gt; /open InfiniteListImpl.java jshell&gt; /open InfiniteList.java

jshell&gt; InfiniteList.iterate(1, x -&gt; x + 1).filter(x -&gt; x % 2 == 1).limit(10).count()

$.. ==&gt; 10

jshell&gt; InfiniteList.iterate(1, x -&gt; x + 1).limit(10).filter(x -&gt; x % 2 == 1).count()

$.. ==&gt; 5

jshell&gt; InfiniteList.iterate(1, x -&gt; x + 1).limit(5).forEach(System.out::println)

1

2

3

4 5

jshell&gt; InfiniteList.iterate(1, x -&gt; x + 1).limit(5).reduce(0, (x, y) -&gt; x + y)

$.. ==&gt; 15

jshell&gt; InfiniteList.iterate(1, x -&gt; x + 1).limit(0).reduce(0, (x, y) -&gt; x + y)

$.. ==&gt; 0

jshell&gt; InfiniteList.iterate(1, x -&gt; x + 1).limit(5).reduce((x, y) -&gt; x + y)

$.. ==&gt; Optional[15]

jshell&gt; InfiniteList.iterate(1, x -&gt; x + 1).limit(0).reduce((x, y) -&gt; x + y)

$.. ==&gt; Optional.empty

jshell&gt; InfiniteList.iterate(1, x -&gt; x + 1).map(x -&gt; x * 2).limit(10).toArray()

$20 ==&gt; Object[10] { 2, 4, 6, 8, 10, 12, 14, 16, 18, 20 }

jshell&gt; InfiniteList.generate(() -&gt; 1).get() | Error:

| cannot find symbol

| symbol: method get()

| InfiniteList.generate(() -&gt; 1).get() | ^——————————–^

jshell&gt; InfiniteList.generate(() -&gt; 1).map(x -&gt; x * 2).get() | Error:

| cannot find symbol

| symbol: method get()

| InfiniteList.generate(() -&gt; 1).map(x -&gt; x * 2).get()

| ^————————————————^

Make a copy of your Java programs to the level directory by typing the Unix commands

$ jar cvf infinite3.jar *.java

$ mkdir infinite3

$ cp *.java infinite3

$ cp infinite3.jar infinite3

Verify your jar archive using

$ jar tf ~/infinite3/infinite3.jar

Level 4

Finally, create the package cs2030.mystream for the InfiniteList interface and its implementation class.

Define a client class Main that imports cs2030.mystream to test your implementation and compile your program using

$ javac -d . *.java

Make a copy of your Java programs to the level directory by typing the Unix commands

$ jar cvf infinite4.jar *.java

$ mkdir infinite4

$ cp *.java infinite4

$ cp infinite4.jar infinite4

Verify your jar archive using

$ jar tf ~/infinite4/infinite4.jar
