/*
Object oriented programming Lab 3 question 1

Complete the Car class by
1.	Declaring the String factory instance variable
2.	Declaring the String model instance variable
3.	Declaring int year instance variable
4.	Declaring string colour instance variable
5.	Writing the constructor method with input parameters for factory, model, year and colour
6.	Writing the method carAge to display the age of the car (2024 - year)
Complete the main method by
1.	Using new to create an instance of Car with the constructor: Car("BMW" , "X5" , 2021 , "Black") 
2.	Printing the car details
3.	Printing the return value for the carAge() method on the Car instance


For example:
Test	Result
Car.main(new String[]{})	Factory = BMW
Model = X5
Year = 2021
Colour = Black
Car Age = 3

Car c= new Car("BMW" , "X5" , 2021 , "Black");
c.model= "X";
System.out.println(c.model);	X
Car c = new Car("BMW" , "X5" , 2021 , "Black");
c.year= 2021;
System.out.println(c.carAge());	3

Car c = new Car("BMW" , "X5" , 2021 , "Black");
c.year= 2019;
System.out.println(c.carAge());	5



public class Car
{
    //declare instance variables here
    
    public static void main(String[] args)
    {
        // Creating instance of Car

        // Printing car details       
       
        
        
        // print in standard output formatting
        // Factory = 
        // Model = 
        // Year = 
        // Colour = 
        // Car Age = 
        
    }

}
*/
public class Car
{
    // 1-4. Declare instance variables
    String factory;
    String model;
    int year;
    String colour;
    
    // 5. Constructor method with input parameters
    public Car(String factory, String model, int year, String colour)
    {
        this.factory = factory;
        this.model = model;
        this.year = year;
        this.colour = colour;
    }
    
    // 6. Method to calculate and return car age
    public int carAge()
    {
        return 2024 - year;
    }
   
    public static void main(String[] args)
    {
        // 1. Creating instance of Car using new
        Car c = new Car("BMW", "X5", 2021, "Black");
        
        // 2. Printing car details in the required format
        System.out.println("Factory = " + c.factory);
        System.out.println("Model = " + c.model);
        System.out.println("Year = " + c.year);
        System.out.println("Colour = " + c.colour);
        
        // 3. Printing the return value for carAge() method
        System.out.println("Car Age = " + c.carAge());
    }
}
