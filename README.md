# Lab 5 – All sorts of sorts

__*Supplied By Instructor*__

---

[TOC]

Write a program to test the bubble, selection, insertion, merge, quick and system sorts. Let ```N=1000``` until they all work then change to ```100000```.

## showArray

The ```showArray``` method should show the first ```10``` and the last ```10``` with ```3``` periods between ```1 2 3 4 5 6 7 8 9 10 ... 89 90 91 92 93 94 95```    --- something like that

## makeArray

The ```makeArray``` method should make random integers from ```1``` to 10000``` ```1245 9876 7844``` --- something like that 

You may (and should) use the resources for the code

## main(String[] args)

```java
public static void main(String[] args) {

    int SIZE = 1000; // change to 100000 when complete       
    int[] list = new int[SIZE];       
    int[] listHold = new int[SIZE];       
    makeArray(list);       
    showArray(list);       
    listHold = list.clone();        
    
    System.out.println("Array size:"+SIZE);       
    
    //bubble      
    
    long startTime = System.nanoTime();        
    
    System.out.println("Bubble sort");        
    
    showArray(list);        
    bubbleSort(list);       
    showArray(list);        
    
    long elapsedTime = System.nanoTime() - startTime;        
    System.out.printf("Time: %3.10f\n",  
    elapsedTime / (Math.pow(10, 9))); 
    
    // ..Selection, Insertion, merge, quick and system sorts
    
} // end main
```

## URL

https://www.toptal.com/developers/sorting-algorithms 