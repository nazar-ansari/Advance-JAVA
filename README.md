# **_Complete JAVA & Advance OOP'S Concept_** ![JAVA](https://cdn-icons-png.flaticon.com/128/226/226777.png) .
<hr>

-  # **_Introduction_**

    ```java
        public class HelloWorld {
        public static void main(String[] args) {
            // Write your code here
        }
     }
     ```
     **_JVM_** (Java Virtual Machine) is an abstract machine that enables your computer to run a Java program.
     Java compiler first compiles your Java code to bytecode. Then, the JVM translates bytecode into native machine code.
     
     ![jvm](https://cdn.programiz.com/sites/tutorial2program/files/how-java-program-runs.jpg)
     
     **_JRE_** (Java Runtime Environment) is a software package that provides Java class libraries, Java Virtual Machine (JVM), and other components that are required to run Java applications.
     
     ![jre](https://cdn.programiz.com/sites/tutorial2program/files/java-realtime-enviornment_0.jpg)
     
     **_JDK_** (Java Development Kit) is a software development kit required to develop applications in Java. When you download JDK, JRE is also downloaded with it.
     
     ![Relation Between Jre jvm jdk](https://cdn.programiz.com/sites/tutorial2program/files/jdk-jre-jvm.jpg)
     
     **Note:** Java is a statically-typed language. It means that all variables must be declared before they can be used.
     
     ```java
            // binary
            int binaryNumber = 0b10010;
            // octal 
            int octalNumber = 027;

            // decimal
            int decNumber = 34;

            // hexadecimal 
            int hexNumber = 0x2F; // 0x represents hexadecimal
            // binary
            int binNumber = 0b10010; // 0b represents binary
            
             double myDouble = 3.4;
             float myFloat = 3.4F;
 
             // 3.445*10^2
             double myDoubleScientific = 3.445e2;

             System.out.println(myDouble);  // prints 3.4
             System.out.println(myFloat);    // prints 3.4
             System.out.println(myDoubleScientific);   // prints 344.5
     ```
     **Logical Operator** :
     ```java
         class Main {
         public static void main(String[] args) {

          // && operator
         System.out.println((5 > 3) && (8 > 5));  // true
         System.out.println((5 > 3) && (8 < 5));  // false

              // || operator
         System.out.println((5 < 3) || (8 > 5));  // true
         System.out.println((5 > 3) || (8 < 5));  // true
         System.out.println((5 < 3) || (8 < 5));  // false

          // ! operator
         System.out.println(!(5 == 3));  // true
         System.out.println(!(5 > 3));  // false
            }
        }
     ```
     **Ternary Operator :**
     ```java
    int februaryDays = 29;
    String result;

    // ternary operator
    result = (februaryDays == 28) ? "Not a leap year" : "Leap year";
    System.out.println(result);
    // THIS IS SINGLE LINE COMMENT
    /*
        THIS IS MULTI LINE COMMENT
    */
     ```
     <hr>
  
 -  # **_Flow-Control_**
 
    ```java
        /*          IF ELSE         */
        
        int number = 0;
        // checks if number is greater than 0
        if (number > 0) {
        System.out.println("The number is positive.");
        }

        // checks if number is less than 0
        else if (number < 0) {
        System.out.println("The number is negative.");
        }
    
        // if both condition is false
        else {
        System.out.println("The number is 0.");
    ```
    ```java
           /*           SWITCH STATEMENT        */
           
          int expression = 9;
           
           switch(expression) {
        
             case 2:
               System.out.println("Small Size");
               break;

             case 3:
               System.out.println("Large Size");
               break;
            
          // default case
          default:
            System.out.println("Unknown Size");
        }
    ```
    ```java
        /*              FOR LOOP        */
        
      int sum = 0;
      int n = 1000;

      // for loop
      for (int i = n; i >= 1; --i) {
          // body inside for loop
        sum += i;     // sum = sum + i
     }
       
        System.out.println("Sum = " + sum);
    ```
    ```java
        /*          FOR-EACH LOOP       */
        
      char[] vowels = {'a', 'e', 'i', 'o', 'u'};
  
      // iterating through an array using the for-each loop
      for (char item: vowels) {
       System.out.println(item);
     }
    ```
    ```java
        /*      WHILE LOOP         */
        
      int i = 1, n = 5;
    
     // while loop from 1 to 5
       while(i <= n) {
        System.out.println(i);
       i++;
     }
    ```
    ```java
        /*          CONTINUE CONCEPT    */
        for (int i = 1; i <= 10; ++i) {

      // if value of i is between 4 and 9
      // continue is executed
      if (i > 4 && i < 9) {
        continue;
      }
      System.out.println(i);
    ```
    <hr>
    
-  # **_Arrays_**
    
    An array is a collection of similar types of data.
    ```java
        //declare and initialize and array
        int[] age = {12, 4, 5, 2, 5};
        
        // declare an array
        int[] age = new int[5];

        // initialize array
        age[0] = 12;
        age[1] = 4;
        age[2] = 5;
        ..             
        
        System.out.println("Using for Loop:");
        for(int i = 0; i < age.length; i++) {
            System.out.println(age[i]);
        }
   
        System.out.println("Using for-each Loop:");
        for(int a : age) {
            System.out.println(a);
        }
    ```
    
    ![Array-Initialization](https://cdn.programiz.com/sites/tutorial2program/files/initialize-array-during-declaration-java.jpg)
    
    **Multidimensional Arrays :**
     
    ![MultiDimensional-Array](https://cdn.programiz.com/sites/tutorial2program/files/java-2d-array.jpg)
     
     ```java
        String[][][] data = new String[3][4][2];
        
        int[][] a = {
            {1, 2, 3}, 
            {4, 5, 6, 9}, 
            {7}, 
        };
      
        // calculate the length of each row
        System.out.println("Length of row 1: " + a[0].length);
        System.out.println("Length of row 2: " + a[1].length);
        System.out.println("Length of row 3: " + a[2].length);
     ```
     ```java
        int[][][] test = {
                {
                  {1, -2, 3}, 
                  {2, 3, 4}
                 }, 
                {
                {-4, -5, 6, 9}, 
                {1}, 
                {2, 3}
                } 
                };  

        // for..each loop to iterate through elements of 3d array
        for (int[][] array2D: test) {
            for (int[] array1D: array2D) {
                for(int item: array1D) {
                    System.out.println(item);
                }
            }
     ```
   **Copy-Arrays :**
   
    ```java
     int [] numbers = {1, 2, 3, 4, 5, 6};
     int [] positiveNumbers = numbers;    // copying arrays
    ```
    *NOTE :* However, there is a problem with this technique. If we change elements of one array, corresponding elements of the other arrays also change
    ```java
        int [] source = {1, 2, 3, 4, 5, 6};
        int [] destination = new int[6];

        // iterate and copy elements from source to destination
        for (int i = 0; i < source.length; ++i) {
            destination[i] = source[i];
        }
      
         // converting array to string
        System.out.println(Arrays.toString(destination));
    ```
    ```java
        int[] n1 = {2, 3, 12, 4, 12, -2};
        int[] n3 = new int[5];
        
        // copying entire n1 array to n2
        System.arraycopy(n1, 0, n2, 0, n1.length);
        System.out.println("n2 = " + Arrays.toString(n2));
    ```
    ```java
        int[] source = {2, 3, 12, 4, 12, -2};
      
        // copying entire source array to destination
        int[] destination1 = Arrays.copyOfRange(source, 0, source.length);      
        System.out.println("destination1 = " + Arrays.toString(destination1));
    ```
    👨‍💻 [TryByRunning](https://www.programiz.com/java-programming/online-compiler)
    
    <hr>
    
-  # **_OOPS_**
    
    **Class & Objects :**
    A class is a blueprint for the object. Before we create an object, we first need to define the class.
    ```java
        class Bicycle {

        // state or field
        private int gear = 5;

        // behavior or method
        public void braking() {
            System.out.println("Working of Braking");
        }
        }
    ```
    An object is called an instance of a class. For example, suppose Bicycle is a class then MountainBicycle, SportsBicycle, TouringBicycle, etc can be considered as objects of the class.
    
     ```java
           className object = new className();

           // for Bicycle class
           Bicycle sportsBicycle = new Bicycle();
           Bicycle touringBicycle = new Bicycle();
     ```
     *NOTE :* Fields and methods of a class are also called members of the class.
     ```java
       class Lamp {
  
    // stores the value for light
    // true if light is on
    // false if light is off
        boolean isOn;
    // method to turn on the light
    void turnOn() {
        isOn = true;
        System.out.println("Light on? " + isOn);
    }

    // method to turnoff the light
    void turnOff() {
        isOn = false;
        System.out.println("Light on? " + isOn);
        }
    }

    class Main {
       public static void main(String[] args) {

        // create objects led and halogen
        Lamp led = new Lamp();
        Lamp halogen = new Lamp();
        // turn on the light by
        // calling method turnOn()
        led.turnOn();
        // turn off the light by
        // calling method turnOff()
        halogen.turnOff();
        }
    }
     ```
     ```java
     OUTPUT:
     Light on? true
     Light on? false
     ```
     ```java
     class Lamp {
     boolean isOn;
     // method to turn on the light
     void turnOn() {}

      public static void main(String[] args) {
    
      // create an object of Lamp
      Lamp led = new Lamp();

     // access method using object
     led.turnOn();
        }
    }
     ```
     
     **Methods :**
     A method is a block of code that performs a specific task.
     ```java
     class Main {

     // method with no parameter
    public void display1() {
        System.out.println("Method without parameter");
    }

    // method with single parameter
    public void display2(int a) {
        System.out.println("Method with a single parameter: " + a);
    }

    public static void main(String[] args) {    
    // create an object of Main
    Main obj = new Main();
    // calling method with no parameter
    obj.display1();        
    // calling method with the single parameter
    obj.display2(24);
        }
    }
     ```
     ```java
     OUTPUT:
     Method without parameter
     Method with a single parameter: 24
     ```
     ```java
         private static int getSquare(int x){
            return x * x;
        }

        public static void main(String[] args) {
            for (int i = 1; i <= 5; i++) {

            // method call
             int result = getSquare(i);
             System.out.println("Square of " + i + " is: " + result);
             }
     ```
     
     **Constructors :**
     A constructor in Java is similar to a method that is invoked when an object of the class is created.
     ```java
     class Main {

        String languages;

        // constructor accepting single value
        Main(String lang) {
            languages = lang;
            System.out.println(languages + " Programming Language");
        }

        public static void main(String[] args) {

            // call constructor by passing a single value
            Main obj1 = new Main("Java");
            Main obj2 = new Main("Python");
            Main obj3 = new Main("C");
            }
        }   
     ```
     ```java
        int a;
        boolean b;

        public static void main(String[] args) {

            // A default constructor is called
            Main obj = new Main();

            System.out.println("Default Value:");
            System.out.println("a = " + obj.a);
            System.out.println("b = " + obj.b);
        }
     ```
     ```java
        OUTPUT:
        Default Value:
        a = 0
        b = false
     ```
     Constructors are invoked implicitly when you instantiate objects .<br>
     A constructor cannot be `abstract` or `static` or `final` .<br>
     A constructor can be overloaded but can not be overridden .<br>
     ```java
       Main() {
        this.language = "Java";
        }

       // constructor with a single parameter
      Main(String language) {
        this.language = language;
        }

    public void getName() {
        System.out.println("Programming Langauage: " + this.language);
    }

    public static void main(String[] args) {

    // call constructor with no parameter
    Main obj1 = new Main();

    // call constructor with a single parameter
    Main obj2 = new Main("Python");

    obj1.getName();
    obj2.getName();
    } 
     ```
     
    **Strings :**
     In Java, a string is a sequence of characters
     ```java
        String greet = "Hello! World";
        System.out.println("String: " + greet);

        // get the length of greet
        int length = greet.length();
     ```
     ```java
        String first = "Java ";
        System.out.println("First String: " + first);

        // create second
        String second = "Programming";
        System.out.println("Second String: " + second);

        // join two strings
        String joinedString = first.concat(second);
     ```
     ```java
        String first = "java programming";
        String second = "java programming";
        String third = "python programming";

        // compare first and second strings
        boolean result1 = first.equals(second);
     ```
     JVM maintains a string pool to store all of its strings inside the memory. The string pool helps in reusing the strings.<br>If the string already exists, the new string is not created. Instead, the new reference, example points to the already existed string (Java).
     ```java
        // creating a char array
        char[] result;
        result = str.toCharArray();
        ----------------------------------------------
        double x=4.22;
        System.out.println(String.valueOf(x));
        ----------------------------------------------
        System.out.println(str1.toUpperCase()); // "LEARN JAVA"
        ----------------------------------------------
        String text = "Java is a fun programming language";
        String[] result = text.split(" ");
        for (String str : result) {
             System.out.print(str + ", ");
        }
        ----------------------------------------------
        int result=text.indexOf("i");
        // getting the index of character 'a'
        // search starts at index 4
        result = str1.indexOf('a', 4);
        System.out.println(str1.charAt(3));
        ----------------------------------------------
        // replace b with c
        System.out.println(str1.replace('b', 'c'));
        ----------------------------------------------
        result = String.join("-", "Java", "is", "fun");
        System.out.println(result);  // Java-is-fun
        ----------------------------------------------
        String str1 = "java is fun";
        System.out.println(str1.substring(0, 4));
        ----------------------------------------------
        boolean result = str1.contains("Java");        
     ```
     **Access-Modifiers :**
     In Java, access modifiers are used to set the accessibility (visibility) of classes, interfaces, variables, methods, constructors, data members, and the setter methods. 
     | **Modifier** | **Description**                                                    |
     | ------------ | ------------------------------------------------------------------ |
     | Default      | declarations are visible only within the package (package private) |
     | Private      | declarations are visible within the class only                     |
     | Protected    | declarations are visible within the package or all subclasses      |
     | Public       | declarations are visible everywhere                                |
     
     Private Access Modifier
     ```java
        class Data {
        // private variable
        private String name;
            }

        public class Main {
        public static void main(String[] main){
        // create an object of Data
        Data d = new Data();
        // access private variable and field from another class
        d.name = "Programiz";
            }
        }
     ```
     ```java
        OUTPUT:
        Main.java:18: error: name has private access in Data
        d.name = "Programiz";
         ^
     ```
     But The Problem Can Be Solved Using `Getters` & `Setters`
     ```java
     class Data {
        private String name;
        // getter method
        public String getName() {
            return this.name;
        }
        // setter method
        public void setName(String name) {
            this.name= name;
        }
    }
    public class Main {
        public static void main(String[] main){
            Data d = new Data();
            // access the private variable using the getter and setter
            d.setName("Programiz");
            System.out.println(d.getName());
            }
        }
     ```
     Protected Access Modifier
     ```java
        class Animal {
        // protected method
        protected void display() {
            System.out.println("I am an animal");
        }
    }

    class Dog extends Animal {
        public static void main(String[] args) {
            // create an object of Dog class
            Dog dog = new Dog();
            // access protected method
            dog.display();
            }
        }
     ```
     *NOTE :* We cannot declare classes or interfaces `protected` in Java.
     
     **This `keyword` :**
     In Java, `this` keyword is used to refer to the current object inside a method or a constructor<br>Mostly , `this` keyword is use to avoid the Ambiguity Between variable for Understanding of Java Compiler .
     ```java
     class Main {
         String name;

        // setter method
        void setName( String name ) {
            this.name = name;
        }

        // getter method
        String getName(){
            return this.name;
        }

        public static void main( String[] args ) {
            Main obj = new Main();
            // calling the setter and the getter method
            obj.setName("Toshiba");
            System.out.println("obj.name: "+obj.getName());
            }
        }
     ```
     we cannot call the constructor explicitly. Instead, we have to use this keyword
     ```java
        class Complex {
            private int a, b;
            // constructor with 2 parameters
            private Complex( int i, int j ){
                this.a = i;
                this.b = j;
            }
            // constructor with single parameter
            private Complex(int i){
                // invokes the constructor with 2 parameters
                this(i, i); 
            }
            // constructor with no parameter
            private Complex(){
                // invokes the constructor with single parameter
                this(0);
            }
            @Override
            public String toString(){
                return this.a + " + " + this.b + "i";
            }
            
            public static void main( String[] args ) {  
                // creating object of Complex class
                // calls the constructor with 2 parameters
                Complex c1 = new Complex(2, 3); 
    
                // calls the constructor with a single parameter
                Complex c2 = new Complex(3);

                // calls the constructor with no parameters
                Complex c3 = new Complex();

                // print objects
                System.out.println(c1);
                System.out.println(c2);
                System.out.println(c3);
            }
        }
     ```
     **Passing This as an Argument**
     ```java
     class ThisExample {
        // declare variables
        int x;
        int y;

        ThisExample(int x, int y) {
            // assign values of variables inside constructor
            this.x = x;
            this.y = y;
            // value of x and y before calling add()
            System.out.println("Before passing this to addTwo() method:");
            System.out.println("x = " + this.x + ", y = " + this.y);

            // call the add() method passing this as argument
            add(this);

            // value of x and y after calling add()
            System.out.println("After passing this to addTwo() method:");
            System.out.println("x = " + this.x + ", y = " + this.y);
        }

        void add(ThisExample o){
            o.x += 2;
            o.y += 2;
            }
        }

    class Main {
        public static void main( String[] args ) {
            ThisExample obj = new ThisExample(1, -2);
            }
        }
     ```
     **Final-Keyword :**
     In Java, the `final` keyword is used to denote constants. It can be used with variables, methods, and classes.
     - The final Variable Cannot be Reinitialized
     - The final method Cannot be Overridden
     - The final Class Cannot be Extended
     
     ```java
     final int AGE=32;
     AGE=44 // Error Cannot Reinitialized
     ```
     ```java
     class FinalDemo {
        // create a final method
        public final void display() {
        System.out.println("This is a final method.");
        }
    }

    class Main extends FinalDemo {
    // try to override final method Will Result in Error
    public final void display() {
        System.out.println("The final method is overridden.");
    }

    public static void main(String[] args) {
        Main obj = new Main();
        obj.display();
        }
    }

     ```
     ```java
     final class FinalClass{
     }
     class Main extends FinalClass{ // Will Result Error
        Main obj = new Main();
        obj.display();
     }     
     ```
     
     **Recursion :**
     A Method Invoking Itself is Called Recursion 
     
     ![Recursion](https://cdn.programiz.com/sites/tutorial2program/files/java-recursive-call.jpg)
     
     **InstanceOf Operator:**
     The `instanceof` operator in Java is used to check whether an object is an instance of a particular class or not.
     ```java
        // Java program to check if an object of a class is also
        //  an instance of the interface implemented by the class

        interface Animal {
        }

        class Dog implements Animal {
        }

        class Main {
            public static void main(String[] args) {

            // create an object of the Dog class
            Dog d1 = new Dog();

            // checks if the object of Dog
            // is also an instance of Animal
            System.out.println(d1 instanceof Animal);  // returns true
            }
        }
     ```
     **Inheritance :**
     The new class that is created is known as subclass (child or derived class) and the existing class from where the child class is derived is known as superclass (parent or base class).
     ```java
        class Animal {

        // field and method of the parent class
        String name;
        public void eat() {
            System.out.println("I can eat");
            }
        }

        // inherit from Animal
        class Dog extends Animal {

        // new method in subclass
        public void display() {
            System.out.println("My name is " + name);
            }
        }

        class Main {
            public static void main(String[] args) {

            // create an object of the subclass
            Dog labrador = new Dog();

            // access field of superclass
            labrador.name = "Rohu";
            labrador.display();

            // call method of superclass
            // using object of subclass
            labrador.eat();
            }
        }
     ```
     
     ![Inheritance-Implementation](https://cdn.programiz.com/sites/tutorial2program/files/java-inheritance-implementation.png)
     
     **super keyword :**
     ```java
     class Animal {

    // method in the superclass
    public void eat() {
        System.out.println("I can eat");
        }
    }

    // Dog inherits Animal
    class Dog extends Animal {

    // overriding the eat() method
    @Override
    public void eat() {

        // call method of superclass
        super.eat();
        System.out.println("I eat dog food");
    }

    // new method in subclass
    public void bark() {
        System.out.println("I can bark");
        }
    }

    class Main {
    public static void main(String[] args) {

    // create an object of the subclass
    Dog labrador = new Dog();

    // call the eat() method
    labrador.eat();
    labrador.bark();
        }
    }
     ```
    **Protected Member In Inheritance :**
    ```java
    class Animal {
        protected String name;

        protected void display() {
            System.out.println("I am an animal.");
            }
        }

    class Dog extends Animal {

        public void getInfo() {
            System.out.println("My name is " + name);
            }
        }

    class Main {
        public static void main(String[] args) {

            // create an object of the subclass
            Dog labrador = new Dog();

            // access protected field and method
            // using the object of subclass
            labrador.name = "Rocky";
            labrador.display();

            labrador.getInfo();
            }
        }
    ```
    ```java
    OUTPUT:
    I am an animal.
    My name is Rocky
    ```
    _**Types of Inheritance**_
    
      Sinle-Inheritance
        
      ![SingleInheritance](https://cdn.programiz.com/sites/tutorial2program/files/java-single-inheritance.png)
        
      MultiLevel-Inheritance
        
      ![Multilevel](https://cdn.programiz.com/sites/tutorial2program/files/java-multilevel-inheritance.png)
        
      Hierarchical-Inheritance
        
      ![HierarchicalInheritance](https://cdn.programiz.com/sites/tutorial2program/files/java-hierarchical-inheritance.png)
        
      Multiple-Inheritance
        
      ![Multiple-Inheritance](https://cdn.programiz.com/sites/tutorial2program/files/java-multiple-inheritance.png)
    
      Hybrid-Inheritance
       
      ![Hybrid-Inheritance](https://cdn.programiz.com/sites/tutorial2program/files/java-hybrid-inheritance.png)
     
     **Method Overriding :**
     We cannot override the method declared as `final` and `static`.
     
     ```java
     class Animal {
        public void displayInfo() {
        System.out.println("I am an animal.");
        }
     }

    class Dog extends Animal {
        public void displayInfo() {
        super.displayInfo();
        System.out.println("I am a dog.");
        }
    }

    class Main {
        public static void main(String[] args) {
        Dog d1 = new Dog();
        d1.displayInfo();
        }
    }
     ```
     **Accessing Attributes of SuperClass :**
     ```java
     class Animal {
        protected String type="animal";
        }

    class Dog extends Animal {
        public String type="mammal";

        public void printType() {
            System.out.println("I am a " + type);
            System.out.println("I am an " + super.type);
            }
        }

    class Main {
        public static void main(String[] args) {
            Dog dog1 = new Dog();
            dog1.printType();
        }
    }

     ```
     ```java
     OUTPUT:
     I am a mammal
     I am an animal
     ```
     **Using SuperClass To Access The Constructors :**
     ```java
     class Animal {

        // default or no-arg constructor of class Animal
        Animal() {
            System.out.println("I am an animal");
            }
        }

    class Dog extends Animal {

        // default or no-arg constructor of class Dog
        Dog() {
            // calling default constructor of the superclass
            super();

            System.out.println("I am a dog");
            }
        }

    class Main {
        public static void main(String[] args) {
            Dog dog1 = new Dog();
            }
        }

     ```
     Calling Parameterized Constructors Using Super() 
     ```java
     class Animal {

        // default or no-arg constructor
        Animal() {
            System.out.println("I am an animal");
        }

        // parameterized constructor
        Animal(String type) {
            System.out.println("Type: "+type);
            }
        }

    class Dog extends Animal {

        // default constructor
        Dog() {

            // calling parameterized constructor of the superclass
            super("Animal");
            System.out.println("I am a dog");
            }
        }

    class Main {
        public static void main(String[] args) {
            Dog dog1 = new Dog();
            }
        }

     ```
     _**Abstract Classed & Methods :**_
     
     The abstract class in Java cannot be instantiated (we cannot create objects of abstract classes). 
     A method that doesn't have its body is known as an abstract method
     
     `abstract void display();`
     
     *NOTE:* `If the abstract class includes any abstract method, then all the child classes inherited from the abstract superclass must provide the implementation of the abstract method`
     > Abstraction is an important concept of object-oriented programming that allows us to hide unnecessary details and only show the needed information.

     > This allows us to manage complexity by omitting or hiding details with a simpler, higher-level idea.
     
     ```java
     abstract class MotorBike {
        abstract void brake();
        }

    class SportsBike extends MotorBike {
    
        // implementation of abstract method
        public void brake() {
            System.out.println("SportsBike Brake");
            }
        }

    class MountainBike extends MotorBike {
    
        // implementation of abstract method
        public void brake() {
            System.out.println("MountainBike Brake");
            }
        }

    class Main {
        public static void main(String[] args) {
            MountainBike m1 = new MountainBike();
            m1.brake();
            SportsBike s1 = new SportsBike();
            s1.brake();
            }
        }
     ```
     ```java
     OUTPUT:
     MountainBike Brake
     SportsBike Brake
     ```
     - An abstract method doesn't have any implementation (method body).
     - We cannot create objects of an abstract class.
     - A subclass must override all abstract methods of an abstract class. 
     
     **Interfaces :**
     
     An interface is a fully abstract class. It includes a group of abstract methods (methods without a body).
     ```java
     interface Polygon {
        void getArea(int length, int breadth);
        }

     // implement the Polygon interface
    class Rectangle implements Polygon {

        // implementation of abstract method
        public void getArea(int length, int breadth) {
            System.out.println("The area of the rectangle is " + (length * breadth));
            }
        }

    class Main {
        public static void main(String[] args) {
            Rectangle r1 = new Rectangle();
            r1.getArea(5, 6);
            }
        }
     ```
     ```java
     OUTPUT:
     The area of the rectangle is 30
     ```
     > *Note:*All the methods inside an interface are implicitly public and all fields are implicitly `public static final` .
     To Implement the body inside the interface we can use the `default` keyword before it .
     ```java
     public default void getSides(){
        //body of getSides()
     }
     ```
     ```java
     // To use the sqrt function
    import java.lang.Math;

    interface  Polygon {
        void getArea();
  
    // calculate the perimeter of a Polygon
    default void getPerimeter(int... sides) {
          int perimeter = 0;
          for (int side: sides) {
            perimeter += side;
        }

    System.out.println("Perimeter: " + perimeter);
        }
    }

    class Triangle implements Polygon {
        private int a, b, c;
        private double s, area;

        // initializing sides of a triangle
        Triangle(int a, int b, int c) {
            this.a = a;
            this.b = b;
            this.c = c;
            s = 0;
        }

    // calculate the area of a triangle
    public void getArea() {
          s = (double) (a + b + c)/2;
          area = Math.sqrt(s*(s-a)*(s-b)*(s-c));
          System.out.println("Area: " + area);
        }
     }

    class Main {
    public static void main(String[] args) {
          Triangle t1 = new Triangle(2, 3, 4);

        // calls the method of the Triangle class
            t1.getArea();

        // calls the method of Polygon
            t1.getPerimeter(2, 3, 4);
            }
        }
     ```
     
     **Polymorphism :**
     
     Polymorphism help us to achieve the consistency in code by using same method for different arguments .
     > NOTE : The print() method is also an example of polymorphism. It is used to print values of different types like char, int, string, etc.
     
     We can Achieve the polymorphism in Two Ways :
      - *Method Overriding*
      - *Method Overloading*
      - ~Operator Overloading~ (Doesn't Support in Java)
     
     ```java
     class Language {
        public void displayInfo() {
            System.out.println("Common English Language");
            }
        }

    class Java extends Language {
        @Override
        public void displayInfo() {
            System.out.println("Java Programming Language");
            }
        }

    class Main {
        public static void main(String[] args) {

            // create an object of Java class
            Java j1 = new Java();
            j1.displayInfo();

            // create an object of Language class
            Language l1 = new Language();
            l1.displayInfo();
            }
        }
     ```
     ```java
     OUTPUT:
     Java Programming Language
     Common English Language
     ```
     Working of JAVA Polymorphism 
     
      ![java-polymorphism](https://cdn.programiz.com/sites/tutorial2program/files/java-polymorphism-implementation.png)
      
      > NOTE : he method that is called is determined during the execution of the program. Hence, method overriding is a `run-time` polymorphism.
      
      ```java
        // method with no arguments
        display() {...}

        // method with a single char type argument
        display(char symbol) {...}
      ```
      > NOTE :  The method that is called is determined by the compiler. Hence, it is also known as `compile-time` polymorphism
      
      > NOTE :  In languages like C++, we can define operators to work differently for different operands. However, Java doesn't support user-defined operator overloading.
      
      **Polymorphic Variable :**
      
      A variable is called polymorphic if it refers to different values under different conditions.
      ```java
     class ProgrammingLanguage {
        public void display() {
            System.out.println("I am Programming Language.");
            }
        }

     class Java extends ProgrammingLanguage {
        @Override
        public void display() {
            System.out.println("I am Object-Oriented Programming Language.");
            }
        }

    class Main {
        public static void main(String[] args) {

            // declare an object variable
            ProgrammingLanguage pl;

            // create object of ProgrammingLanguage
            pl = new ProgrammingLanguage();
            pl.display();

            // create object of Java class
            pl = new Java();
            pl.display();
            }
        }
      ```
      ```java
      I am Programming Language.
      I am Object-Oriented Programming Language.
      ```
      **Encapsulation :**
      
      It prevents outer classes from accessing and changing fields and methods of a class. This also helps to achieve data hiding.
      ```java
      class Area {

        // fields to calculate area
        int length;
        int breadth;

        // constructor to initialize values
        Area(int length, int breadth) {
            this.length = length;
            this.breadth = breadth;
        }

        // method to calculate area
        public void getArea() {
            int area = length * breadth;
            System.out.println("Area: " + area);
            }
        }

    class Main {
        public static void main(String[] args) {

            // create object of Area
            // pass value of length and breadth
            Area rectangle = new Area(5, 6);
            rectangle.getArea();
            }
        }
      ```
      > NOTE :  People often consider encapsulation as data hiding, but that's not entirely true.Encapsulation refers to the bundling of related fields and methods together. This can be used to achieve data hiding. Encapsulation in itself is not data hiding.

      ```java
      class Person {

        // private field
        private int age;

        // getter method
        public int getAge() {
            return age;
        }

        // setter method
        public void setAge(int age) {
            this.age = age;
            }
        }

    class Main {
        public static void main(String[] args) {

            // create an object of Person
            Person p1 = new Person();

            // change age using setter
            p1.setAge(24);

            // access age using getter
            System.out.println("My age is " + p1.getAge());
            }
        }
      ```
      Making `age` private allowed us to restrict unauthorized access from outside the class. This is **data hiding** .
