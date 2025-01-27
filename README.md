# Difference-Arrays-ArrayLists
// Differences between Arrays and ArrayLists.

// In Java, arrays are used to store multiple items of the same type in one place. They have a fixed size, meaning you decide how many items they can hold when you create them. However, once the number of items is set, such cannot be changed. Arrays allow you to access items directly using their position (index).

// ArrayLists, on the other hand, are more flexible. They can grow or shrink as you add or remove items, so their size does not need to be known beforehand. They also come with built-in features, like methods to easily add, remove, or search for items. Unlike arrays, which can store primitive types (like int), ArrayLists can only hold objects, though Java can convert primitives into objects automatically.

// The main difference between arrays and ArrayList is that arrays are simple, fixed in size, and better for performance, while ArrayLists are easier to use and more flexible, making them great when the number of items can change.

// This program demonstrates the main differences between Arrays and ArrayLists.
import java.util.ArrayList;

public class ArraysVsArrayList {
    public static void main(String[] args) {
     
        // 1. Arrays are fixed in size, so you must define the size when creating them.
        // 2. Arrays can store primitives (like int, char) or objects.
        
        // Array Example
        String[] arrayExample = new String[3]; // Array of size 3
        arrayExample[0] = "Avocado";
        arrayExample[1] = "Banana";
        arrayExample[2] = "Pumpkin";

        // Print elements of the array.
        System.out.println("Array Elements:");
        for (int i = 0; i < arrayExample.length; i++) {
            System.out.println(arrayExample[i]);
        }

        // 1. ArrayLists are dynamic and grow or shrink as needed.
        // 2. ArrayLists can only store objects (no primitives).
        // 3. ArrayLists provide useful methods like add(), remove(), and size().

        // ArrayList Example
        ArrayList<String> arrayListExample = new ArrayList<>();
        arrayListExample.add("Dog"); // Adding an element.
        arrayListExample.add("Cat");
        arrayListExample.add("Bird");

        // Add another element to show dynamic growth.
        arrayListExample.add("Fish");

        // Print elements of the ArrayList.
        System.out.println("\nArrayList Elements:");
        for (int i = 0; i < arrayListExample.size(); i++) {
            System.out.println(arrayListExample.get(i));
        }
    }
}
