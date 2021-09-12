# Java

Java is an Object Oriented Programming language.

Few Points about Java Concepts

1. when a method is called in java. it is called by value. it means Java call a method by its value not by it's reference.

  Ex 1: 
      Person p = new Person("Mike");
      Person p2 = new Person("Rezene");
      
      changeTheNameOfTheObject(p);
      swapTheTwoObject(p,p2);
      
      Sytem.out.println(p.name);
      System.out.println(p2.name);
      
      
      public static void changeTheNameOfTheObject(p){
      
        p.setName("John");
      }
      
      public static void swapTheTwoObject(p , p2){
        Person temp = p;
        p = p2;
        p2 = temp;
      }
      
      
      //The Result for this code is going to be
      
      John
      Rezene
      
      The reson for this is since the ChangeName method is accessing the value it can access the method within the object
      however the swap method is trying to change the reference of the object while we are passing the copy of the reference. which 
      means we are passing the value of the object so it is impossible to change the reference with a parameter that we pass.
      
      
      
      



























