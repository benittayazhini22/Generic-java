import java.util.*; 

class genericMaximum  

{ 

   public static <T extends Comparable<T>> T findMax(T[] data)  

    { 

        T max = data[0]; 

        for (int i = 1; i < data.length; i++)  

        { 

            if (data[i].compareTo(max) > 0)  

            { 

              max = data[i]; 

            } 

        } 

        return max; 

    } 

   public static void main(String[] args)  

    { 

        Integer[] numbers = {10, 23, 34, 5, 47}; 

        Float[] values = {10.4f, 25.6f, 17.9f, 40.8f}; 

        String[] names = {"apple", "mango", "orange", "banana"}; 

        System.out.println("Maximum integer = " + findMax(numbers)); 

        System.out.println("Maximum Float = " + findMax(values)); 

        System.out.println("Maximum String = " + findMax(names)); 

    } 

} 
 # Generic-java
