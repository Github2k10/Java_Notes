# Part-7: Collections

**1. Why do we need Collections in Java?**
> *Answer:* Collections are an essential part of Java programming as they provide a way to store and manipulate groups of objects efficiently. They offer a flexible, reusable, and easy-to-use solution for storing and managing data in a program. <br>
> Collection provide efficient storage and retrieval, dynamic data structures, polymorphism, and standardized interfaces that's make collections important part of Java programming.

<br> <b>

 
**2. What are the important interfaces in the Collection Hierarchy?**
> *Answer:* The most important interface in the collection hierarchy are: <br>
> 1. Collection Interface: This is the root interface of the java collection framework. It defines the basic methods that all Collections should have, such as add(), remove(), and size(), etc. <br>
> 2. List Interface: The List interface extends the Collection inter face and provides an ordered collection of elements that can contain duplicates. It allows elements to be added or removed at any position in the list. <br>
> 3. Set Interface. The Set interface extends the Collection interface and provides an unordered collection of elements that cannot contain duplicates. <br>
> 4. Queue Interface: The Queue interface extends the Collection interface and provides a collection of elements that supports operations like enqueues and dequeue. It is typically used to implement data structures like queues and stacks. <br>
> 5. Map Interface: The Map interface represents a mapping between a set of keys and a set of values. It does not extend the Collection interface. <br>
> 6. Iterator Interface: The Iterator Interface is used to iterate over elements in a collection. It provides methods like hasNext() and next() to traverse elements in the collection.

<br> <br>

  **3. What are the important methods that are declared in the Collection Interface?**
> *Answer:* Some of the important methods that are declared in the Collection Interface are: <br>
> 1. add(E e): This method adds the specified element to the collection. <br>
> 2. addAll(Collection<? extends E> c): This method adds all the elements from the specified collection to the current collection. <br>
> 3. clear(): This method removes all elements from the collection. <br>
> 4. contains(Object o): This method returns true if the collection contains the specified element. <br>
> 5. containsAll(Collection<?> c): This method returns true if the collection contains all elements in the specified collection. <br>
> 6. equals(Object o): This method compares the current collection with the specified object for equality. <br>
> 7. hasCode(): This method returns the hash code value of the collection. <br>
> 8. isEmpty(): This method returns true if the collection is empty. <br>
> 9. remove(Object o): This method removes the specified element from the collection. <br>
> 10. removeAll(Collection<?> c): This method removes all the elements from the collection that are also present in the specified collection. <br>
> 11. size(): This method returns the number of elements in the collection. <br>
> 12. toArray(): This method returns an array containing all elements in the collection. <br>
> 13. toArray(T[] a): This method returns an array containing all elements in the collection, using the specified array if it is large enough; otherwise, a new array is allocated. 

<br> <br>

**4. Can you explain briefly about the List Interface?**
> *Answer:* List in Java provides the facility to maintain the ordered collection. It contains the index-based methods to insert, update, delete, and search the elements. It can have the duplicate elements also. We can also store the null elements in the list. <br>
> The List interface is found in the java.util package and inherits the Collection interface. It is a factor of ListIterator interface. Through the ListIterator, we can iterate the list in forward and backward directions. The implementation classes of List interface are ArrayList, LinkedList, Stack and Vector. <br>
> List Interface declaration: public interface List<E> extends Collection<E> <br> <br>
> Some of the important methods that are declared int the List interface are add(int, E element), get(int index), indexOf(Object o), lastIndexOf(Object o), remove(int index), set(int index, E element), subList(int from index, int index).

<br> <br>

**5. Explain about ArrayList with an example?**
> *Answer:* Java ArrayList class uses a dynamic array for storing the elements. It is like an array, but there is no size limit. We can add or remove elements anytime. So, it is much more flexible than the traditional array. <br>
> The ArrayList in Java can have the duplicate elements also. It implements the List interface, so we can use all the methods or the List interface here. The ArrayList maintains the insertion order internally. <br> <br>
> The important points about the Java ArrayList class are: 
> - It can contain duplicate elements.
> - It maintains insertion order.
> - It is non synchronized.
> - It allows random access because the array works on an index basis.
> - Manipulation is a little bit slower than the LinkedList in java because a lot of shifting needs to occur if any element is removed from teh array list.  <b> <br>
> Syntax: List<Integer> list = new ArrayList<>(); <br>
> Example: <br> <br>
> import java.util.*;  <br>
> public class ArrayListExample1{  <br>
> public static void main(String args[]){  <br>
> ArrayList<String> list=new ArrayList<String>();  //Creating arraylist    <br>
>      list.add("Java");//Adding object in arraylist    <br>
>     list.add("HTML");    <br>
>      list.add("CSS");    <br>
>      list.add("JavaScript");    <br>
>      //Printing the arraylist object  <br>   
>      System.out.println(list);  <br>
>  }  <br>
> }  

<br> <br>

**6. Can an ArrayList have Duplicate elements?**
> *Answer:* Yes, ArrayList can have duplicate elements. 

<br> <b>

**7. How do you iterate around an ArrayList using Iterator?**
> *Answer:* Here is an example of how we can iterate around an ArrayList: <br> <br>
> import java.util.ArrayList; <br>
> import java.util.Iterator; <br>
> public class ArrayListIteratorExample { <br>
> public static void main(String[] args) { <br>
> ArrayList<String> list = new ArrayList<String>(); <br>
> list.add("Java"); <br>
> list.add("JavaScript"); <br>
> list.add("HTML"); <br>
>  <br>
> Iterator<String> iterator = list.iterator(); <br>
> while (iterator.hasNext()) { <br>
> String fruit = iterator.next(); <br>
> System.out.println(fruit); <br>
> } <br>
> } <br>
> } <br> <br>
> Output: <br>
> Java <br>
> JavaScript <br>
> HTML 

<br> <br>

**8. How do you sort an ArrayList?**
> *Answer:* To sort an ArrayList in Java we can use sort() method of Collections framework, we can use Comparable interface, we can use comparator interface, we can also use sorting algorithms, etc. <br>
> Here are the example of sorting an ArrayList using sort() method of Collections framework <br> <br>
> import java.util.ArrayList; <br>
> import java.util.Collections; <br> <br>
> public class ArrayListSortExample { <br>
> public static void main(String[] args) { <br>
> ArrayList<Integer> numbers = new ArrayList<Integer>(); <br>
> numbers.add(5); <br>
> numbers.add(3); <br>
> numbers.add(9); <br>
> numbers.add(1); <br> <br>
> Collections.sort(numbers); <br> <br>
> for (int number : numbers) { <br>
> System.out.print(number + " "); <br>
> } <br>
> } <br>
> } <br>
> Output: 1 3 5 9

<br> <br>

**9. How do you sort elements in an ArrayList using Comparable interface?**
> *Answer:8* Here is the example to sort an ArrayList using Comparable interface <br> <br>
> import java.util.ArrayList; <br>
> import java.util.Collections; <br>
>  <br>
> public class ArrayListComparableExample { <br>
> public static void main(String[] args) { <br>
> ArrayList<Student> students = new ArrayList<Student>(); <br>
> students.add(new Student(5, "Alice")); <br>
> students.add(new Student(3, "Bob")); <br>
> students.add(new Student(9, "Charlie")); <br>
> students.add(new Student(1, "David")); <br>
>  <br>
> Collections.sort(students); <br>
>  <br>
> for (Student student : students) { <br>
> System.out.println(student.getId() + " " + student.getName()); <br>
> } <br>
> } <br>
> } <br>
>  <br>
> class Student implements Comparable<Student> { <br>
> private int id; <br>
> private String name; <br>
>  <br>
> public Student(int id, String name) { <br>
> this.id = id; <br>
> this.name = name; <br>
> } <br>
>  <br>
> public int getId() { <br>
> return id; <br>
> } <br>
>  <br>
> public String getName() { <br>
> return name; <br>
> } <br>
>  <br>
> public int compareTo(Student student) { <br>
> return this.id - student.id; <br>
> } <br>
> } <br> <br>
> Output: <br>
> 1 David <br>
> 3 Bob <br>
> 5 Alice <br>
> 9 Charlie 

<br> <br>

**10. How do you sort elements in an ArrayList using Comparator interface?**
> *Answer:* Here is the example to sort an ArrayList using Comparator interface: <br> <br>
> import java.util.ArrayList; <br>
> import java.util.Collections; <br>
> import java.util.Comparator; <br>
>  <br>
> public class ArrayListComparatorExample { <br>
> public static void main(String[] args) { <br>
> ArrayList<Student> students = new ArrayList<Student>(); <br>
> students.add(new Student(5, "Alice")); <br>
> students.add(new Student(3, "Bob")); <br>
> students.add(new Student(9, "Charlie")); <br>
> students.add(new Student(1, "David")); <br>
>  <br>
> StudentComparator studentComparator = new StudentComparator(); <br>
> Collections.sort(students, studentComparator); <br>
>  <br>
> for (Student student : students) { <br>
> System.out.println(student.getId() + " " + student.getName()); <br>
> } <br>
> } <br>
> } <br>
>  <br>
> class Student { <br>
> private int id; <br>
> private String name; <br>
>  <br>
> public Student(int id, String name) { <br>
> this.id = id; <br>
> this.name = name; <br>
> } <br>
>  <br>
> public int getId() { <br>
> return id; <br>
> } <br>
>  <br>
> public String getName() { <br>
> return name; <br>
> } <br>
> } <br>
>  <br>
> class StudentComparator implements Comparator<Student> { <br>
> public int compare(Student s1, Student s2) { <br>
> return s1.getName().compareTo(s2.getName()); <br>
> } <br>
> } <br> <br>
> Output: <br>
> 5 Alice <br>
> 3 Bob <br>
> 9 Charlie <br>
> 1 David 

<br> <br>

**11. What is Vector class? How is it different from an ArrayList?**
> *Answer:* Vector is like the dynamic array (ArrayList) which can grow or shrink its size. We can store n-number of elements in it as there is no size limit. It is a part of Collection framework since Java 1.2. It implements the List interface. <br>
> It is recommended to use Vector class in the thread-safe implementation only. If we don't need to use the thread-safe implementation, we should use the ArrayList. <br>
> Here are some points that make Vector class different from an ArrayList: <br>
> 1. Vector is synchronized. <br>
> 2. Java Vector contains many legacy methods that are not part of a collection's framework. <br>
> 3. Vector is thread-safe that means multiple threads can access and modify a Vector object concurrently without causing any data corruption or inconsistency issues. <b>
> 4. ArrayList is generally faster than Vector because it is not synchronized by default.

<br> <b>

**12. What is LinkedList? What interfaces does it implement? How is it different from an ArrayList?**
> *Answer:* LinkedList is another implementation of the List interface in java, which is used to store a sequence of elements in a linked list data structure. In a linked list, each element is stored as a node that contains a reference to the next node in the list. This makes it easy to add or remove elements from the list, but it can also incur a performance penalty compared to arrays for certain types of operations. <br>
> In addition to the List interface, LinkedList also implements the Deque interface, which provides methods for adding or removing elements from ends of the list. <br> <br>
> Here are some of the differences between LinkedList and ArrayList in Java: 
> 1. ArrayList is generally faster than LinkedList for random access and iteration operations because it provides direct access to elements using an index.
> 2. ArrayList is more efficient for random access operations, while LinkedList is more efficient for adding or removing elements in the middle of the list. <br>
> 3. ArrayList is generally faster than LinkedList for random access and iteration operations because it provides direct access to elements using an index. 
> 4. ArrayList uses a contiguous block of memory to store elements, which can lead to wasted space it the initial capacity is too high, or if elements are removed from the middle of the list. In contrast, LinkedList only uses as much memory as necessary to store the nodes and their references.

<br> <br>

**13. Can you briefly explain about the Set Interface?**
> *Answer:* The Set interface in Java is part of the java.util package and is used to store a collection of unique elements. In other words, a Set can contain no duplicate elements. The Set interface extends the Collection interface and adds a few extra methods to ensure uniqueness and provide additional functionality for dealing with sets. The elements in a Set are not ordered in any particular way. Set implementations are optimized for fast membership testing, which means we can quickly check if an element is present in the set or not. <br>
> Example: <br> <br>
> import java.util.*;   <br>
> public class setExample{   <br>
> public static void main(String[] args)   <br>
> {<br>
> Set<String> data = new LinkedHashSet<String>();   <br>
> <br>
> data.add("Java");   <br>
> data.add("HTML");   <br>
> data.add("JavaScript");   <br>
> data.add("Java");   <br>
> <br>
> System.out.println(data);   <br>
> }   <br>
> }   <br> <br>
> Output: <br>
> [Java, HTML, JavaScript]

<br> <br>

**14. What are the important interfaces related to the Set Interface?**
> *Answer:* 'SortedSet', 'NavigableSet', 'HashSet', 'TreeSet', and 'LinkedHashSet' are the related to the Set interface. 

<br> <br>

**15. What is the difference between Set and SortedSet interfaces?**
> *Answer:* <br>
> | Set | SortedSet |
> | --- | --------- |
> | Elements are not stored in sorted order. | Elements are stored in sorted order. |
> | Set interface extend by SortedSet | SortedSet interface extends Set interface. |
> | It has several implementations, including 'HashSet', 'TreeSet', and 'LinkedHashSet'. | Only one implementation 'TreeSet' | 

<br> <br>

**16. Can you give examples of classes that implement the Set Interface?**
> *Answer:* 'HashSet', 'TreeSet', 'LinkedHashSet', and 'EnumSet' are the classes that implement the Set interface. 

<br> <br>

**17. What is a HashSet?**
> *Answer:* 'HashSet' is a class in Java that implements the 'Set' interface, and is used to store a collection of unique elements in no particular order. It is implemented using hash table, which allows for constant-time performance for the basic operations like 'add()', 'remove()', and 'contains()'. <br>
> The 'HashSet' class internally uses a 'HashMap' object to store the elements, where the keys of the 'HashMap' are the elements in the 'HashSet', and the values are dummy objects. The 'add()' method of 'HashSet' simply calls the 'put()' method of the underlying 'HashMap' with the elements as the key and the dummy object as the value. The 'remove()' and 'contains()' methods similarly call the corresponding methods of the underlying 'HashMap'. <br>
> Example: <br>
> Set<String> set = new HashSet<>(); <br>
> set.add("Java"); <br>
> set.add("HTML"); <br>
> set.add("CSS"); <br>
> set.add("JavaScript"); <br>
> System.out.println(set); // Output: [CSS, HTML, Java, JavaScript]

<br> <br>

**18. What is a TreeSet? How is different from a HashSet?**
> *Answer:* 'TreeSet' is a class in Java implements the 'SortedSet' interface, and is used to store a collection of unique elements in a sorted order defined by their natural ordering or a custom 'Comparator'. It is implemented using a self-balancing binary search tree, which allows for log(n) time performance for basic operation like 'add()', 'remove()', and 'contains()', where n is the number of the elements in the set. <br>
> The main difference between 'TreeSet' and 'HashSet' is that 'TreeSet' maintains a sorted order of the elements, while 'HashSet' does not maintain any particular order. This makes 'TreeSet' useful when we need to store elements in a sorted manner. <br>
> Example: <br>
> Set<Integer> set = new TreeSet<>();
> set.add(3);
> set.add(1);
> set.add(5);
> set.add(2);
> System.out.println(set); // Output: [1, 2, 3, 5]

<br> <br>

**19. Can you give examples of implementations of NavigableSet?**
> *Answer:* 'TreeSet', 'ConcurrentSkipListSet', 'SubSet', and 'DescendingSet' are the examples of implementations of NavigableSet. 

<br> <br>

**20. Explain briefly about Queue Interface?**
> *Answer:* The 'Queue' interface in Java represents a collection that is designed to hold elements in a specific order for processing. It is similar to list, but with additional operations that support queue-like behavior. Specifically, a queue allows elements to be added to end, and removed from the other end, following a first-in, first-out (FiFO) ordering. The 'Queue' interface extends the 'Collection' interface, and adds several methods for enqueue and dequeue elemets, as well as for inspecting the head and tail of the queue. <br>
> The 'PriorityQueue', 'LinkedList', and 'PriorityBlockingQueue' are the implementations of 'Queue' interface.

<br> <br>

**21. Can you briefly explain about the Map Interface?**
> *Answer:* The 'Map' interface in Java represents a collection of key-value pairs, where each key is associated with a value. It is similar to a dictionary or an associated keys, and supports operations for adding, updating, and removing key-value paris.  <br>
> The 'Map' interface extends the 'Collection' interface, but unlike other collection interfaces, it defines two type parameters, one for the key type and one for the value type. <br>
> put(K key, V value), get(Object key), remove(Object key), containsKey(Object k), etc. are the important methods declared in the 'Map' interface. <br>
> 'HashMap', 'LinkedHashMap', and 'TreeMap' are the implementation of the 'Map' interface. A Map can't be traversed, so we need to convert it into Set using keySet() or entrySet() method.

<br> <br>

**22. What is difference between Map and SortedMap?**
> *Answer:* The main difference between 'Map' and 'SortedMap' interfaces in java is that 'SortedMap' guarantees that the keys in the map are sorted in ascending order according to their natural ordering or a specified comparator. 'SortedMap' is an interface of the 'Map' interface and adds additional methods that supports the ordering of keys, such as 'firstKey()', 'lastKey()', 'subMap()', etc.

<br> <br>

**23. What is a HashMap?**
> *Answer:* 'HashMap' is a class in Java that implements the 'Map' interface to store key-value pairs. It provides constant-time performance for basic operation such as inserting, removing, and retrieving elements. Internally, 'HashMap' uses an array and a hash function to store the key value pairs and to locate elements quickly based on their key. The hash function generates an integer hash code for each key, which is used to compute the index of the corresponding entry in the array. <br>
> 'HashMap' allows null values for both keys and values, and it is not synchronized, meaning that it is not thread-safe by default. However, it can be made thread-safe by using the 'Collections.synchronizedMap()' method, which returns a synchronized version of the map. <br>
> Example: <br>
> Map<Integer, String> map = new HashMap<>(); <br>
> map.put(1, "java");
> map.put(2, "HTML");
> map.put(3, "CSS");
> map.get(2); // Output: HTML

<b> <br>

**24. What are the different methods in a Hash Map?**
> *Answer:* Here are some of the commonly used methods of HashMap: <br>
> 1. 'put(K Key, V value)': this is used to associate the specified value with a specified key in the map, or it will update the value if the key already exists. <br>
> 2. 'get(Object o)': it will return the value associated with the specified key in the map or return null it key is not there. <br>
> 3. 'remove(Object key)': remove the key-value pair with a specified key from the map, and return the key-value pair. If the key is not there, it will return null. <br>
> 4. 'containsKey(Object key)': returns 'true' if key present in the map else returns 'false'. <br>
> 5. 'containsValue(Object Value)': return 'true' if the value present in the map, it will return 'false'. <br>
> 6. 'size()': it returns the number of key-value pairs in the map. <br>
> 7. 'isEmpty()': returns 'true' if the map is empty, else returns 'false'. <br>
> 8. 'keySet()': returns a 'Set' containing all the keys in the map. <br>
> 9. 'values()': returns a 'Collections' containing all the values in the map. <br>
> 10. 'entrySet()': returns a 'Set' containing all the key-value pairs in the map as 'Map.Entry' object. <br>
> There are other methods present in the HashMap such as 'clear()', 'putAll()', 'replace()', and more. 

<br> <br>

**25. What is a TreeMap? How is different from a HashMap?**
> *Answer:* 'TreeMap' is a class in java that implements the 'SortedMap' interface and stores key-value pairs in a sorted order based on the natural ordering of the kys or a custom 'Comparator'. It uses a self-balancing binary search tree to maintain the keys in sorted order, which allows for efficient search, insertion, and deletion operations with a time complexity of O(log n), where n is the number of key-value pairs in the map. <br>
> The main difference between 'TreeMap' and 'HashMap' is that 'TreeMap' maintains the keys in the sorted order, while 'HashMap' does not specify any order of the keys. And typically 'HashMap' provides faster performance than 'TreeMap'.
