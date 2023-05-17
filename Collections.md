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
