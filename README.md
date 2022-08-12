# **_Complete JAVA & Advance OOP'S Concept_** ![JAVA](https://cdn-icons-png.flaticon.com/128/226/226777.png) .
<hr>

- ## **_Introduction_**

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
  
 - ## **_Flow-Control_**
 
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
    
- ## **_Arrays_**
    
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
    
    
    