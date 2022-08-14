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
     
    
    