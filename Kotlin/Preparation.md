# Kotlin

#### Q1. The code snippet compile and runs without issue, but does not wait for the coroutine to show the "there" message. Which line of code will cause the code to wait for the coroutine to finish before exiting?

```kotlin
fun main() = runBlocking {
    val task = GlobalScope.launch {
        delay(1000L)
        println("there")
    }
    println("Hello,")
}
```

- [ ] `task.complete()`
- [ ] `task.wait()`
- [ ] `task.join()`
- [ ] `task.cancel()`

#### Q2. You would like to group a list of students by last name and get the total number of groups. Which line of code accomplishes this, assuming you have a list of the Student data class?

```kotlin
data class Student(val firstName: String, val lastName: String)
```

- [ ] `println(students.groupBy{ it.lastName }.count())`
- [ ] `println(students.groupBy{ it.lastName.first() }.fold().count())`
- [ ] `println(students.groupingBy{ it.lastName.first() }.count())`
- [ ] `println(students.groupingBy{ it.lastName.first() }.size())`

#### Q3. Kotlin interfaces ad abstract classes are very similar. What is one thing abstract class can do that interfaces cannot?

- [ ] Only abstract classes are inheritable by subclasses
- [ ] Only abstract classes can inherit from multiple superclasses
- [ ] Only abstract classes can have abstract methods
- [ ] Only abstract classes can store state
      

#### Q4. Your application has an **add** function. How could you use its **invoke** methods and display the results?

```kotlin
fun add(a: Int, b: Int): Int {
  return a + b
}
```

- [ ] `println(add(5,10).invoke())`
- [ ] `println(::add.invoke(5, 10))`
- [ ] `println(::add.invoke{5, 10})`
- [ ] `println(add.invoke(5,10))`

#### Q5. What is the entry point for a Kotlin application?

- [ ] `fun static main(){}`
- [ ] `fun main(){}`
- [ ] `fun Main(){}`
- [ ] `public static void main(){}`

#### Q6. You are writing a console app in Kotlin that processes test entered by the user. If the user enters an empty string, the program exits. Which kind of loop would work best for this app? Keep in mind that the loop is entered at least once

- [ ] a do..while loop ([reference](https://kotlinlang.org/docs/control-flow.html#while-loops))
- [ ] a for loop
- [ ] a while loop
- [ ] a forEach loop

#### Q7. You pass an integer to a function expecting type Any. It works without issue. Why is a primitive integer able to work with a function that expects an object?

```kotlin
fun showHashCode(obj: Any){
  println("${obj.hasCode()}")
}
fun main() {
  showHashCode(1)
}
```

- [ ] While the code runs, it does not produce correct results
- [ ] The integer is always a class
- [ ] The compiler runs an implicit `.toClass()` method on the integer
- [ ] The integer is autoboxed to a Kotlin Int class

#### Q8. You have started a long-running coroutine whose job you have assigned to a variable named **task**. If the need arose, how could you abort the coroutine?

```kotlin
val task = launch {
  // long running job
}
```

- [ ] `task.join()`
- [ ] `task.abort()`
- [ ] `job.stop()`
- [ ] `task.cancel()`

#### Q9. You are attempting to assign an integer variable to a long variable, but Kotlin compiler flags it as an error. Why?

- [ ] You must wrap all implicit conversion in a try/catch block
- [ ] You can only assign `Long` to an `Int`, not the other way around
- [ ] There is no implicit conversion from `Int` to `Long` ([reference](https://kotlinlang.org/docs/basic-types.html#explicit-conversions))
- [ ] All integers in Kotlin are of type `Long`

#### Q10. You have written a snippet of code to display the results of the roll of a six-sided die. When the die displays from 3 to 6 inclusive, you want to display a special message. Using a Kotlin range, what code should you add?

```kotlin
when (die) {
  1 -> println("die is 1")
  2 -> println("die is 2")
  ___ -> printlin("die is between 3 and 6")
  else -> printlin("dies is unknown")
}
```

- [ ] `3,4,5,6`
- [ ] `in 3..6`
- [ ] `3 : 6`
- [ ] `{3,4,5,6}`

#### Q11. The function **typeChecker** receiver a parameter **obj** of type **Any**. Based upon the type of **obj**, it prints different messages for Int, String, Double, and Float types; if not any of the mentioned types, it prints "unknown type". What operator allows you to determine the type of an object?

- [ ] `instanceof`
- [ ] `is` 
- [ ] `typeof`
- [ ] `as`

#### Q12. This code does not print any output to the console. What is wrong?

```kotlin
firstName?.let {
  println("Greeting $firstname!")
}
```

- [ ] A null pointer exception is thrown
- [ ] `firstName` is equal to `null` 
- [ ] `firstName` is equal to an empty string
- [ ] `firstName` is equal to Boolean `false`

#### Q13. You have a function simple() that is called frequently in your code. You place the inline prefix on the function. What effect does it have on the code?

```kotlin
inline fun simple(x: Int): Int{
  return x * x
}
fun main() {
  for(count in 1..1000) {
    simple(count)
  }
}
```

- [ ] The code will give a stack overflow error
- [ ] The compiler warns of insignificant performance impact 
- [ ] The compiler warns of significant memory usage
- [ ] The code is significantly faster

#### Q14.How do you fill in the blank below to display all of the even numbers from 1 to 10 with least amount of code?

```kotlin
for (_____) {
  println("There are $count butterflies.")
}
```

- [ ] `count in 1..10`
- [ ] `count in 2..10 step 2` 
- [ ] `count in 1..10 % 2`
- [ ] `var count=2; count <= 10; count+=2`

#### Q15. What value is printed by println()?

```kotlin
val set = setOf("apple", "pear", "orange", "apple")
println(set.count())
```

- [ ] 3 
- [ ] 4
- [ ] 1
- [ ] 5

#### Q16. Which line of code shows how to display a nullable string's length and shows 0 instead of null?

- [ ] `println(b!!.length ?: 0)`
- [ ] `println(b?.length ?: 0)`
- [ ] `println(b?.length ?? 0)`
- [ ] `println(b == null? 0: b.length)`

#### Q17. In the file main.kt, you ae filtering a list of integers and want to use an already existing function, removeBadValues. What is the proper way to invoke the function from filter in the line below?

```kotlin
val list2 = (80..100).toList().filter(_____)
```

- [ ] `::removeBadValues` 
- [ ] `GlobalScope.removeBadValues()`
- [ ] `Mainkt.removeBadValues`
- [ ] `removeBadValues`

#### Q18. Which code snippet correctly shows a for loop using a range to display "1 2 3 4 5 6"?

- [ ] `for(z in 1..7) println("$z ")`
- [ ] `for(z in 1..6) print("$z ")` 
- [ ] `for(z in 1 to 6) print("$z ")`
- [ ] `for(z in 1..7) print("$z ")`

#### Q19. You are upgrading a Java class to Kotlin. What should you use to replace the Java class's static fields?

- [ ] an anonymous object
- [ ] a static property
- [ ] a companion object 
- [ ] a backing field

#### Q20. Which function changes the value of the element at the current iterator location?

- [ ] `change()`
- [ ] `modify()`
- [ ] `set()` 
- [ ] `assign()`

#### Q21. You would like to print each score on its own line with its cardinal position. Without using **var** or **val**, which method allows iteration with both the value and its position?

```kotlin
fun main() {
  val highScores = listOf(4000, 2000, 10200, 12000, 9030)
}
```

- [ ] `.withIndex()`
- [ ] `.forEachIndexed()`
- [ ] `.forEach()`
- [ ] `.forIndexes()`

#### Q22. From the Supervisor subclass, how do you call the Employee class's display() method?

```kotlin
open class Employee(){
  open fun display() = println("Employee display()")
}
class Supervisor : Employee() {
  override fun display() {
    println("Supervisor display()")
  }
}
```

- [ ] `Employee.display() `
- [ ] `::display()`
- [ ] `super.display()` 
- [ ] `override.display()`

#### Q23. The code below compiled and executed without issue before the addition of the line declaring errorStatus. Why does this line break the code?

```kotlin
sealed class Status(){
  object Error : Status()
  class Success : Status()
}
fun main(){
  var successStatus = Status.Success()
  var errorStatus = Status.Error()
}
```

- [ ] `StatusError` is an object, not a class and cannot be instantiated 
- [ ] Only one instance of the class `Status` can be instantiated at a time
- [ ] `Status.Error` must be declared as an immutable type
- [ ] `Status.Error` is pribate to class and cannot be declared externally

#### Q24. The code below is expected to display the numbers from 1 to 10, but it does not. Why?

```kotlin
val seq = sequence { yieldAll(1..20) }
  .filter { it < 11 }
  println(seq)
```

- [ ] You cannot assign a sequence to a variable
- [ ] To produce result, a sequence must have terminal operation. In this case, it needs a `.toList()` ([reference]
- [ ] The `.filter{ it < 11 }` should be `.filter{ it > 11 }`
- [ ] The `yieldAll(1..20)` should be `yieldAll(1..10)`

#### Q25. What three methods does this class have?

```kotlin
class Person
```

- [ ] `equals(), hashCode(), and toString()` 
- [ ] `equals(), toHash(), and super()`
- [ ] `print(), println(), and toString()`
- [ ] `clone(), equals(), and super()`

#### Q26. What will happen when you try to build and run this code snippet?
```kotlin
class SpecialFunction : () -> Unit {
  override fun invoke() {
    println("Invoked from an instance.")
  }
}
fun main() {
  try { SpecialFunction()() }
  catch (ex: Exception) { println("An error occurred") }
}
```
- [ ] A syntax error occurs due to the line `SpecialFunction()()`.
- [ ] The message "An Error occurred" is displayed.
- [ ] The message "Invoked from an instance." is displayed. // the second "()" is equals to .invoke()
- [ ] A compile error occurs. You cannot override the `invoke()` method.

#### Q27. Which statement declares a variable mileage whose value never changes and is inferred to be an integer?
- [ ] `val mileage:Int = 566`
- [ ] `var mileage:Int = 566`
- [ ] `val mileage = 566` 
- [ ] `const int mileage = 566`

#### Q28. You have two arrays, a and b. Which line combines a and b as a list containing the contents of both?
```kotlin
val a = array0f(1, 2, 3)
val b = array0f(166,266,366)
```
- [ ] `val c = a + b`
- [ ] `val c = list0f(a, b)`
- [ ] `val c = list0f(*a, *b)` 
- [ ] `val c = list0f(a+b)`

#### Q29. What is the preferred way to create an immutable variable of type long?
- [ ] `var longInt = 10L`
- [ ] `const long longInt = 10`
- [ ] `val longInt = 10L`
- [ ] `val longInt:Long = 10`

#### Q30. Which line converts the binaryStr, whish contain only 0s and 1s, to an integer representing its decimal value?
```kotlin
val binaryStr = "00001111"
```
- [ ] `val myInt = toInt(binaryStr)`
- [ ] `val myInt = binaryStr.toInt("0b")`
- [ ] `val myInt = binaryStr.toInt()`
- [ ] `val myInt = binaryStr.toInt(2)`

#### Q31. In a Kotlin program, which lines can be marked with a label
- [ ] `Any program line can be marked with a label`
- [ ] `Any statement can be marked with a label`
- [ ] `Any expression can be marked with a lable`
- [ ] `Only the beginning of loops can be marked with a label`

#### Q32. Which is the proper way to declare a singleton named DatabaseManager?

- [ ] `object DatabaseManager {}` 
- [ ] `singleton DatabaseManager {}`
- [ ] `static class DatabaseManager {}`
- [ ] `data class DatabaseManager {}`


#### Q33. Your function is passed by a parameter obj of type Any. Which code snippet shows a way to retrieve the original type of obj, including package information?

- [ ] `obj.classInfo()`
- [ ] `obj.typeInfo()`
- [ ] `obj::class.simpleName`
- [ ] `obj::class` 

#### Q34. Which is the correct declaration of an integer array with a size of 5?

- [ ] `val arrs[5]: Int`
- [ ] `val arrs = IntArray(5)` 
- [ ] `val arrs: Int[5]`
- [ ] `val arrs = Array<Int>(5)`

#### Q35. You have created a class that should be visible only to the other code in its module. Which modifier do you use?

- [ ] `internal` 
- [ ] `private`
- [ ] `public`
- [ ] `protected`

#### Q36. Kotlin has two equality operators, == and ===. What is the difference?

- [ ] `==` determines if two primitive types are identical. `===` determines if two objects are identical
- [ ] `==` determines if two references point to the same object. `===` determines if two objects have the same value
- [ ] `==` determines if two objects have the same value. `===` determines if two strings have the same value
- [ ] `==` determines if two objects have the same value. `===` determines if two references point to the same object

#### Q37. Which snippet correctly shows setting the variable max to whichever variable holds the greatest value, a or b, using idiomatic Kotlin?

- [ ] `val max3 = a.max(b)` 
- [ ] `val max = a > b ? a : b`
- [ ] `val max = if (a > b) a else b`
- [ ] `if (a > b) max = a else max = b`

#### Q38. You have an enum class Signal that represents the state of a network connection. You want to print the position number of the SENDING enum. Which line of code does that?

```java
enum class Signal { OPEN, CLOSED, SENDING }
```

- [ ] `println(Signal.SENDING.position())`
- [ ] `println(Signal.SENDING.hashCode())`
- [ ] `println(Signal.SENDING)`
- [ ] `println(Signal.SENDING.ordinal)` 

#### Q39. In order to subclass the Person class, what is one thing you must do?

```kotlin
abstract class Person(val name: String) {
  abstract fun displayJob(description: String)
}
```

- [ ] The subclass must be marked sealed
- [ ] You must override the `displayJob()` method 
- [ ] You must mark the subclass as final
- [ ] An abstract class cannot be extended, so you must change it to open

#### Q40. The code snippet below translates a database user to a model user. Because their names are both User, you must use their fully qualified names, which is cumbersome. You do not have access to either of the imported classes' source code. How can you shorten the type names?

```kotlin
import com.tekadept.app.model.User
import com.tekadept.app.database.User
class UserService{
  fun translateUser(user: com.tekadept.app.database.User): User =
    com.tekadept.app.model.User("${user.first} ${user.last}")
}
```

- [ ] Use import as to change the type name 
- [ ] Create subtypes with shorter names
- [ ] Create interfaces with shorter names
- [ ] Create extension classes with shorter names

#### Q41. Both const and @JvmField create constants. What can const do that @JvmField cannot?

```java
class Detail {
  companion object {
    const val COLOR = "Blue"
    @JvmField val SIZE = "Really Big"
  }
}
```

- [ ] `const` is compatible with Java, but `@JvmField` is not
- [ ] The compiler will inline const so it is faster and more memory efficient 
- [ ] Virtually any type can be used with const but not `@JvmField`
- [ ] const can also be used with mutable types

#### Q42. You have a when expression for all of the subclasses of the class Attribute. To satisfy the when, you must include an else clause. Unfortunately, whenever a new subclass is added, it returns unknown. You would prefer to remove the else clause so the compiler generates an error for unknown subtypes. What is one simple thing you can do to achieve this?

```kotlin
open class Attribute
class Href: Attribute()
class Src: Attribute()
class Alt: Attribute()
fun getAttribute(attribute: Attribute) : String {
  return when (attribute) {
    is Href -> "href"
    is Alt -> "alt"
    is Src -> "src"
    else -> "unknown"
  }
}
```

- [ ] Replace `open` with `closed`
- [ ] Replace `open` with `sealed` 
- [ ] Replace `open` with `private`
- [ ] Replace `open` with `public`

#### Q43. You would like to know each time a class property is updated. Which code snippet shows a built-in delegated property that can accomplish this?

- [ ] `Delegates.watcher()`
- [ ] `Delegates.observable()` 
- [ ] `Delegates.rx()`
- [ ] `Delegates.observer()`

#### Q44. Why doesn't this code compile?

```kotlin
val addend = 1
infix fun Int.add(added: Int=1) = this + addend
fun main(){
  val msg = "Hello"
  println( msg shouldMatch "Hello")
  println( 10 multiply 5 + 2)
  println( 10 add 5)
}
```

- [ ] infix function must be marked public
- [ ] In Kotlin, add is a keyword
- [ ] Extension functions use `it`, not `this`, as the default parameter name
- [ ] infix functions cannot have default values 

#### Q45. What is the correct way to initialize a nullable variable?

- [ ] `val name = null`
- [ ] `var name: String`
- [ ] `val name: String`
- [ ] `val name: String? = null`

#### Q46. Which line of code is a shorter, more idiomatic version of the displayed snippet?

```kotlin
val len: Int = if (x != null) x.length else -1
```

- [ ] `val len = x?.let{x.len} else {-1}`
- [ ] `val len = x!!.length ?: -1`
- [ ] `val len:Int = (x != null)? x.length : -1`
- [ ] `val len = x?.length ?: -1`

#### Q47. You are creating a Kotlin unit test library. What else should you add to make the following code compile without error?

```kotlin
fun String.shouldEqual(value: String) = this == value
fun main(){
  val msg = "test message"
  println(msg shouldEqual "test message")
}
```

- [ ] The extension function should be marked public
- [ ] Add the prefix operator to the shouldMatch extension function
- [ ] The code is not legal in Kotlin (should be `println(msg.shouldEqual("test message"))`)
- [ ] Add the prefix infix to the shouldMatch extension function

#### Q48. What is the difference between the declarations of COLOR and SIZE?

```kotlin
class Record{
  companion object {
    const val COLOR = "Red"
    val SIZE = "Large"
  }
}
```

- [ ] Since `COLOR` and `SIZE` are both immutable, they are identical internally
- [ ] Both are immutable, but the use of the keyword const makes `COLOR` slower and less space efficient than `SIZE`
- [ ] const makes `COLOR` faster, but not compatible with Java. Without const, `SIZE` is still compatible with Java
- [ ] Both are immutable, but the use of the keyword const makes `COLOR` faster and more space efficient than `SIZE` 

#### Q49. Why does not this code snippet compile?

```kotlin
class Cat (name: String) {
  fun greet() { println("Hello ${this.name}") }
}
fun main() {
  val thunderCat = Cat("ThunderCat")
  thunderCat.greet()
}
```

- [ ] Because name is a class parameter, not a property-it is unresolved `main()`.
- [ ] In order to create an instance of a class, you need the keyword `new`
- [ ] The reference to name needs to be scoped to the class, so it should be `this.name`
- [ ] Classes cannot be immutable. You need to change `var` to `val`

#### Q50. The code below shows a typical way to show both index and value in many languages, including Kotlin. Which line of code shows a way to get both index and value more idiomatically?

```kotlin
var ndx = 0;
for (value in 1..5){
  println("$ndx - $value")
  ndx++
}
```

- [ ] `for( (ndx, value) in (1..20).withIndex() ){` 
- [ ] `for( (ndx, value) in (1..20).pair() ){`
- [ ] `for( Pair(ndx, value) in 1..20 ){`
- [ ] `for( (ndx, value) in *(1..20) ){`

#### Q51. Inside an extension function, what is the name of the variable that corresponds to the receiver object

- [ ] The variable is named **it**
- [ ] The variable is named **this**
- [ ] The variable is named **receiver**
- [ ] The variable is named **default**

#### Q52. The Kotlin .. operator can be written as which function?

- [ ] `a.from(b)`
- [ ] `a.range(b)`
- [ ] `a.rangeTo(b)`
- [ ] `a.to(b)`

#### Q53. How can you retrieve the value of the property codeName without referring to it by name or destructuring?

```kotlin
data class Project(var codeName: String, var version: String)
fun main(){
  val proj = Project("Chilli Pepper", "2.1.0")
}
```

- [ ] `proj.0`
- [ ] `proj[0]`
- [ ] `proj[1]`
- [ ] `proj.component1()`

#### Q54. This function generates Fibonacci sequence. Which function is missing?

```kotlin
fun fibonacci() = sequence {
  var params = Pair(0, 1)
  while (true) {
    ___(params.first)
    params = Pair(params.second, params.first + params.second)
  }
}
```

- [ ] `with()`
- [ ] `yield()` 
- [ ] `skip()`
- [ ] `return()`

#### Q55. In this code snippet, why does the compiler not allow the value of y to change?

```kotlin
for(y in 1..100) y+=2
```

- [ ] `y` must be declared with `var` to be mutable
- [ ] `y` is an implicitly immutable value
- [ ] `y` can change only in a while loop
- [ ] In order to change `y`, it must be declared outside of the loop

#### Q56. This code snippet compiles without error, but never prints the results when executed. What could be wrong?

```kotlin
val result = generateSequence(1) { it + 1 }.toList()
println(result)
```

- [ ] The sequence lacks a terminal operation. 
- [ ] The sequence is infinite and lacks an intermediate operation to make `it` finite.
- [ ] The expression should begin with `generateSequence(0)`.
- [ ] The `it` parameter should be replaced with `this`.

#### Q57. An error is generated when you try to compile the following code. How should you change the call to printStudents to fix the error?

```kotlin
fun main() {
    val students = arrayOf("Abel", "Bill", "Cindy", "Darla")
    printStudents(students)
}
fun printStudents(vararg students: String) {
    for(student in students) println(student)
}
```

- [ ] `printStudents(students.toList())`
- [ ] `printStudents(students!!)`
- [ ] `printStudents(*students)`
- [ ] `printStudents(students[])`

#### Q58. Both y and z are immutable references pointing to fixed-size collections of the same four integers. Are there any differences?

```kotlin
val y = arrayOf(10, 20, 30, 40)
val z = listOf(10, 20, 30, 40)
```

- [ ] You can modify the contents of the elements in `y` but not `z`.
- [ ] There are not any differences. `y` and `z` are a type alias of the same type.
- [ ] You add more elements to `z` since it is a list.
- [ ] You can modify the contents of the elements in `z` but not `y`.

#### Q59. Class BB inherits from class AA. BB uses a different method to calculate the price. As shown, the code does not compile. What changes is needed to resolve the compilation error?

```kotlin
open class AA() {
     var price: Int = 0
        get() = field + 10
}
class BB() : AA() {
     var price: Int = 0
        get() = field + 20
}
```

- [ ] You need to add a lateinit modifier to `AA.price`.
- [ ] You simply need to add an override modifier to `BB.price`.
- [ ] You need to add an open modifier to `AA.price` and an override modifier to `BB.price`.
- [ ] You need to add a public modifier to `AA.price` and a protected modifier to `BB.price`.

#### Q60. What is the output of this code?

```kotlin
val quote = "The eagle has landed."
println("The length of the quote is $quote.length")
```

- [ ] The length of the quote is The eagle has landed.
- [ ] A compilation error is displayed.
- [ ] The length of the quote is `21`
- [ ] The length of the quote is `The eagle has landed..length`

#### Q61. You have an unordered list of high scores. Which is the simple method to sort the highScores in descending order?

```kotlin
fun main() {
    val highScores = listOf(4000, 2000, 10200, 12000, 9030)
```
- [ ] `.sortedByDescending()`
- [ ] `.descending()`
- [ ] `.sortedDescending()`
- [ ] `.sort("DESC")`
#### Q62. Your class has a property name that gets assigned later. You do not want it to be a nullable type. Using a delegate, how should you declare it?
- [ ] `lateinit var name: String` // lateinit is modifier not delegate
- [ ] `var name: String by lazy`
- [ ] `var name: String by Delegates.notNull()`
- [ ] `var name: String? = null`
#### Q63. You want to know each time a class property is updated. If the new value is not within range, you want to stop the update. Which code snippet shows a built-in delegated property that can accomplish this?
- [ ] `Delegates.vetoable()`
- [ ] `Delegates.cancellable()`
- [ ] `Delegates.observer()`
- [ ] `Delegates.watcher()`
#### Q64. Which line of code shows how to call a Fibonacci function, bypass the first three elements, grab the next six, and sort the elements in descending order?
- [ ] `val sorted = fibonacci().skip(3).take(6).sortedDescending().toList()`
- [ ] `val sorted = fibonacci().skip(3).take(6).sortedByDescending().toList()`
- [ ] `val sorted = fibonacci().skip(3).limit(6).sortedByDescending().toList()`
- [ ] `val sorted = fibonacci().drop(3).take(6).sortedDescending().toList()` 
#### Q65. You have two arrays, a and b. Which line combines a and b as a list containing the contents of both?
```kotlin
val a = arrayOf(1, 2, 3)
val b = arrayOf(100, 200, 3000)
```
- [ ] `val c = list of (a, b)`
- [ ] `val c = a + b`
- [ ] `val c = listOf(a+b)`
- [ ] `val c = listOf(*a, *b)` 
#### Q66. This code is occasionally throwing a null pointer exception (NPE). How can you change the code so it never throws as NPE?
```kotlin
println("length of First Name = ${firstName!!.length}")
```
- [ ] Replace `!!.` with `?.` 
- [ ] Replace `!!.` with `?:.`
- [ ] Surround the line with a try/catch block.
- [ ] Replace `!!.` with `?.let`.
#### Q67. What is the execution order of init blocks and properties during initialization?
- [ ] All of the properties are executed in order of appearance, and then the init blocks are executed.
- [ ] The init blocks and properties are executed in the same order they appear in the code. 
- [ ] All of the init blocks are executed in order of appearance, and then the properties are executed.
- [ ] The order of execution is not guaranteed, so code should be written accordingly.
#### Q68. Both const and @JvmField create constants. What can @JvmField do that const cannot?
```kotlin
class Styles {
  companion object {
    const val COLOR = "Blue"
      @JvmField val SIZE = "Really big"
   }
}
```
- [ ] `const` works only with strings and primitives. `@JvmField` does not have that restriction. 
- [ ] `@JvmField` works as a top-level variable, but `const` works only in a class.
- [ ] `@JvmField` is compatible with Java, but `const` is not.
- [ ] `@JvmField` is always inlined for faster code.
#### Q69. What are the two ways to make a coroutine's computation code cancellable? 
- [ ] Call the `yield()` function or check the `isActive` property.
- [ ] Call the `cancelled()` function or check the `isActive` property.
- [ ] Call the `stillActive()` function or check the `isCancelled` property.
- [ ] Call the `checkCancelled()` function or check the `isCancelled` property.
#### Q70. Given the code below, how can you write the line this.moveTo("LA") more concisely?
```kotlin
data class Student (val name: String, var location: String) {
  fun moveTo (newLoc: String) { location = newLoc }
}
fun main() {
  Student ("Snow", "Cologne").run {
  this.moveTo ("LA")
}
```
- [ ] `moveTo( "LA")`
- [ ] `::moveTo("LA")`
- [ ] `moveTo("LA")`
- [ ] `it.moveTo("LA")`
#### Q71. For the Product class you are designing, you would like the price to be readable by anyone, but changeable only from within the class. Which property declaration implements your design?
- [ ] Option 1
```
var price: Int = 0
  public get()
  private set
```
- [ ] Option 2 
```
var price: Int = 0
  private set
```
- [ ] Option 3
```
var price: Int = 0
  val set
```
- [ ] Option 4
```
val price: Int=0
```
#### Q72. When the **Airplane** class is instantiated, it displays **Aircraft = null**, not **Aircraft = C130** why?
```kotlin
abstract class Aircraft {
  init { println("Aircraft = ${getName()}") }
  abstract fun getName(): String
}
class Airplane(private val name: String) : Aircraft() {
  override fun getName(): String = name
}
```
- [ ] Classes are initialized in the same order they are in the file, therefore, Aircraft should appear after Airplane
- [ ] The code needs to pass the parameter to the base class's primary constructor. Since it does not, it receives a null
- [ ] Abstract function always returns null
- [ ] A superclass is initialized before its subclass. Therefore, name has not been set before it is rendered
#### Q73. Your code need to try casting an object. If the cast is not possible, you do not want an exception generated, instead you want null to be assigned. Which operator can safely cast a value?
- [ ] `as?` 
- [ ] `??`
- [ ] `is`
- [ ] `as`
#### Q74. Kotlin will not compile this code snippet. What is wrong?
```kotlin
class Employee
class Manager : Employee()
```
- [ ] In order to inherit from a class, it must be marked **open** 
- [ ] In order to inherit from a class, it must be marked **public**
- [ ] In order to inherit from a class, it must be marked **sealed**
- [ ] In order to inherit from a class, it must be marked **override**
#### Q75. You have created a data class, Point, that holds two properties, x and y, representing a point on a grid. You want to use the hash symbol for subtraction on the Point class, but the code as shown will not compile. How can you fix it?
```kotlin
data class Point(val x: Int, val y: Int)
operator fun Point.plus(other: Point) = Point(x + other.x, y + other.y)
operator fun Point.hash(other: Point) = Point(x - other.x, y - other.y)
fun main() {
    val point1 = Point(10, 20)
    val point2 = Point(20, 30)
    println(point1 + point2)
    println(point1 # point2)
}
```
- [ ] You cannot; the hash symbol is not a valid operator.
- [ ] You should replace the word hash with octothorpe, the actual name for the symbol.
- [ ] You should use `minus` instead of hash, then type alias the minus symbol. // Note: How can you fix it?
- [ ] You need to replace operator with the word `infix`.

#### Q76. All classes in Kotlin inherit from which superclass?
- [ ] `Default`
- [ ] `Super`
- [ ] `Any` 
- [ ] `Object`

#### Q77. You have created an array to hold three strings. When you run the code below, the compiler displays an error. Why does the code fail?

```kotlin
val names = arrayOf<String>(3)
names[3] = "Delta"
```

- [ ] `Arrays use zero-based indexes. The value 3 is outside the array's bounds`
- [ ] `You accessed the element with an index but should have used .set()`
- [ ] `You declared the array with val but should have used var`
- [ ] `You cannot change the value of an element of an array. You should have used a mutable list`

#### Q78. You have written a function, sort(), that should accept only collections that implement the `Comparable` interface. How can you restrict the function?

```kotlin
fun sort(list: List<T>): List <T> {
    return list.sorted()
}
```

- [ ] `Add <T -> Comparable<T>> between the `fun` keyword and the function name`
- [ ] `Add Comparable<T> between the `fun` keyword and the function name`
- [ ] `Add <T : Comparable<T>> between the `fun` keyword and the function name`
- [ ] `Add <T where Comparable<T>> between the `fun` keyword and the function name`

#### Q79. Kotlin classes are final by default. What does final mean?


- [ ] final means that you cannot use interfaces with this class.
- [ ] final means that this is the only file that can use the class.
- [ ] final means that you cannot extend the class.
- [ ] final classes cannot be used in the finally section of a try/catch block.

#### Q79. You have created an array to hold three strings. When you run the code bellow, the compiler displays an error. Why does the code fail?
```
val names = arrayOf<String>(3)
names[3]= "Delta"
```
- [ ] Arrays use zero-based indexes. The value 3 is outside of the array's bounds
- [ ] You accessed the element with an index but should have used.set().
- [ ] You declared the array with val but should have used var
- [ ] You cannot changes the value of an element of an array. You should have used a mutable list.
