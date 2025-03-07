# Java-Assignment-010 - Classes and Objects

## Part 1 - Analyze
* Add Comments to the Code below and label the following:
  1. Class name 
     - Student
  2. All **instance variables/fields** and their data-types 
     - name (date-type is String) and rollNo (data-type is int)
  3. The **Constructor** and the **Constructor Parameters** 
     - Student(String s, int r), Parameters are s (String, name of student) and r (int, the number the student rolled)
  4. Where a **Student** object gets created. 
     - Line 29?
  5. Where the **instance variables** value gets set and what its values are. 
     - The constructor assigns name = s and rollNo = r
  6. All the instance methods for the class **Student**
     - I'm gonna guess its .methodForDisplay... 

```java
class Student{ //Class Name
    private String name; //name (date-type is String)
    private int rollNo; //rollNo (data-type is int)
   
    Student(String s, int r) //Constructor
    { //values get set here
   	    name = s; 
   	    rollNo = r;
    }
   
    void methodForDisplay()
    {
        System.out.println(name+"'s Roll No: "+rollNo);
    }

    public static void main(String[] args) {
        Student obj1 = new Student("Rambo",21); //Object gets created here
        //Here is also where the values are passed as parameters, where r and s get their values
        obj1.methodForDisplay();
    }
}
```

## Part 2 - Public VS Static

* Read the W3Schools page on class methods: [W3Schools Java Class Methods](https://www.w3schools.com/java/java_class_methods.asp)
* In your own words, write a few sentences below explaining the difference between static and public methods in relation to a class.
  - Static and Public are both modifiers for a class. Static methods can be accessed without creating an object, whereas Public methods can only be accessed by objects.
## Part 3 - Dogs

* View the image below, and from the image, construct a Java file **Dog** that mirrors the diagrammed class and the 3 dog objects.
![Dog Class](images/ClassVSObject.png)

* Your class should be named **Dog**
* You should have **private** instance variables/fields for all the data members.
* You should have a **constructor** that sets the initial state of the data members via passed parameters.
    * Think about what data-types the fields and parameters will need!!!
* You should have 4 instance methods for eat, run, sleep, and name
* You should have a **main** method that creates the 3 Dog objects in the diagram.
* Make at least 2 of your methods functional (i.e. perform some action)!!!
    * For Example: method eat might take a class parameter named **Food** (i.e. another class) that has a field **weight**, and your eat method might reduce the weight in **Food**.

## Part 4 - Turn-In

* Commit your code and push it back to your account.
* Create a Pull request as you have been doing for all assignments.
* Paste the Pull request URL back into the Canvass assignment page for credit.
