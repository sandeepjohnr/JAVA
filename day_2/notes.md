# Day 2

        class xyz{
            public static void main(String[]args){
                System.out println("start");  
                xyz.createOTP();
                System.out println("start"); 

            }
            public static void createOTP(){
                System.out println("OTP created");
            }
        }

## Method
method is a set of statement which is used to perform a specific task. to execute method statement calling a method is compilsory. main method is called by JRE.

if we create public class in java file then the file name should be same as class name.  
we can create any number of default classes in java file but we can not create more than one public class 
       
        class x{
                    public static void main(String[]args){
                        System.out println("start");  
                        xyz.createOTP();
                        System.out println("start"); 

                    }
        }

        class y{
            public static void main(String[]args){
                System.out println("start");  
                xyz.createOTP();
                System.out println("start"); 

            }
        }

for the above code can be in the same file but when compled there will different bytecode generated for both class seperatly  
 

## Variables
 it is a container which is used to store value  
 java is strictly typed programming language (which means data-type is used while creating the variable )  

### syntax
        data type varname;

        varname = value;

example code:  
        class xyz{
            public static void main(String[]args){
                int age; decleration  
                age = 23; initilization  
                System.out println("start");  

            }
        }

redeclaration of a variable is not possible in java  
example:  
        int n = 10;
        System.out.println(n);
        int n = 20; // REdecleration - which will throw an error   
        System.out.println(n);  


        int n = 10;
        System.out.println(n);
        n = 20; // reinitilization which is acceptable 
        System.out.println(n);
## Data Type
there are two types of datatype 

|Data Type|
|primitive|non-primitive|
|byte|String|
|short|class name|
|int|array|
|long|object|
|float||
|double||
|char||
|boolean||



|data type|size|
|byte|1byte|
|short|2byte|
|int|4byte|
|long|8byte|
|float|4byte|
|double|8byte|
|char|2byte|
|boolean|1byte|
 

in java char has 2byte because it supports unicode  
