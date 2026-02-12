# Java

Java is a High-level programing langauge.    
this means it can be easily understood by humans and it is closer to english  
it has simple syntax.
java is a object orianted  
it is platform independent("write once, run anywhere")  

## How does java works?  
ones the java code is written (source code) and compiled there will be a creation of .class file (byte code). this .class file is unreadable by humans only a machine can understand this. 
to excicute a java file javac file.java -> (creation of .class file) -> java file -> output 

		public class Main {  
	    public static void main(String[] args) {  
	        System.out.println("Hello World");  
	    }  
	}    

## public class main:  
class = Blueprint  
main = class name   

## public static void main(String[] args)  
all the execution starts from main  
to print or display an output we use:  
			
		system.out.println()  

println = print + move to next line  
print = print on same line  



	public class Main {

	    static void greet() {
	        System.out.println("Hello Sandeep!");
	    }
	
	    public static void main(String[] args) {
	        System.out.println("Inside main method");
	        
	        greet();  
	  	  }
	}  

    

