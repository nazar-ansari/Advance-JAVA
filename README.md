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