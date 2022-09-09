# Set Lab

## Learning Goals

- Create and use Sets

## Instructions

Write a program that prompts the user for different cities around the world.
Since a city only exists once, we want to make sure the user does not enter
duplicate city names. This is another great use case for our `Set` interface.

Follow the given instructions and tips:

- Create a `GlobalDirectory` class.
  - Use a `Set` of `String` objects to keep track of the cities the user has
    already entered.
  - If a city has been added to the `Set`, relay that back to the user with the
    message "<city> has been added!"
  - If a city cannot be added to the `Set` because it would result in a duplicate
    city, then tell the user "Oops - <city> is already in the set."
  - When prompted, iterate through the set to show each city in the directory.
- Finish writing the `DirectoryDriver` class.
  - The `printMenu()` method has already been written with how program should be
    driven.
  - Write the `main()` method to execute the driver class and test the
    `GlobalDirectory` class.

## Starter Code

Consider the starter code in the driver class. Note that the driver class is
not finished. You will need to write the `main()` method to prompt the user.

```java
 class DirectoryDriver {
    public static void main(String[] args) {
        // Your code here
    }

    public static void printMenu() {
        System.out.println("Welcome to the Global Directory! What would you like to do?");
        System.out.println("0. Exit");
        System.out.println("1. Add a City to the Directory");
        System.out.println("2. Show the Cities in the Directory");
        System.out.println();
    }
}
```

## Sample Output

Here is an example run of the code for your reference. Make sure your output
looks the same when given these values:

```plaintext
Welcome to the Global Directory! What would you like to do?
0. Exit
1. Add a City to the Directory
2. Show the Cities in the Directory

1
What is the name of the city you would like to add?
Colorado Springs, CO
Colorado Springs, CO has been added!

Welcome to the Global Directory! What would you like to do?
0. Exit
1. Add a City to the Directory
2. Show the Cities in the Directory

1
What is the name of the city you would like to add?
Colorado Springs, CO
Oops - Colorado Springs, CO is already in the set.

Welcome to the Global Directory! What would you like to do?
0. Exit
1. Add a City to the Directory
2. Show the Cities in the Directory

1
What is the name of the city you would like to add?
Portland, Oregon
Portland, Oregon has been added!

Welcome to the Global Directory! What would you like to do?
0. Exit
1. Add a City to the Directory
2. Show the Cities in the Directory

1
What is the name of the city you would like to add?
Phoenixville, PA
Phoenixville, PA has been added!

Welcome to the Global Directory! What would you like to do?
0. Exit
1. Add a City to the Directory
2. Show the Cities in the Directory

2
Phoenixville, PA
Portland, Oregon
Colorado Springs, CO

Welcome to the Global Directory! What would you like to do?
0. Exit
1. Add a City to the Directory
2. Show the Cities in the Directory

0

```
