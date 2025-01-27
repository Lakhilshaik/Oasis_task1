# Oasis_task1
Number Guessing Game 1234567
<br>
hi guyrs
<br>
// Online Java Compiler
<br>
// Use this editor to write, compile and run your Java code online

import java.util.Scanner;
import java.util.Random;
class a{
    static Random r=new Random();
      static  Scanner sc=new Scanner(System.in);
    static int level1(){
      
       
        int attempts=0;
        int score=0;
          System.out.println("<-----------------RULES------------------>");
             System.out.println("YOU HAVE 5 ATTEMPTS YOU HAVE SCORE MINIMUN 3 TO ENTER INTO LEVEL 2");
        
        
        if(attempts<=5){
           for(int i=1;i<=5;i++){
                 int n=r.nextInt(10);
                  System.out.println(n);
                 System.out.println("Enter Your Guessed Number between  1 to 10");
                 int GuessingNum=sc.nextInt();
                 if(GuessingNum==n){
                     System.out.println("You Guessed right num");
                     attempts++;
                     score++;
                 }
                else if(GuessingNum>n){
                     System.out.println("Guessed num is higher than generated num");
                     attempts++;
                 }
                 else if(GuessingNum<n){
                     System.out.println("Guessed num is lower than generated num");
                     attempts++;
                     
                 }
                 else{
                     System.out.println("YOU entered number out of range");
                 }
            }
            System.out.println("your score is "+score);
             System.out.println("And you had completed  "+ attempts+" attempts");
        
    }
        return score;
    }
    static int level2(){
         
         int attempts=0;
        int score=0;
         System.out.println("<-----------------RULES------------------>");
             System.out.println("<----YOU HAVE 5 ATTEMPTS YOU HAVE SCORE MINIMUN 3 TO ENTER INTO LEVEL 3---->");
        
        
        if(attempts<=5){
            for(int i=1;i<=5;i++){
                 int n=r.nextInt(20);
 System.out.println(n);
                 System.out.println("<----Enter Your Guessed Number from 1 between 20---->");
                 int GuessingNum=sc.nextInt();
                 if(GuessingNum==n){
                     System.out.println("<----You Guessed right num---->");
                     attempts++;
                     score++;
                 }
                else if(GuessingNum>n){
                     System.out.println("<----Guessed num is higher than generated num---->");
                     attempts++;
                 }
                 else if(GuessingNum<n){
                     System.out.println("<----Guessed num is lower than generated num---->");
                     attempts++;
                     
                 }
                 else{
                     System.out.println("<----YOU entered number out of range---->");
                 }
            }
            System.out.println("your score is----> "+score);
             System.out.println("<----And you had completed "+ attempts+" attempts---->");
        }
        return score;
    }
    static void level3(){
        
         
           System.out.println("<-----------------RULES------------------>");
         System.out.println("<----YOU HAVE 5 ATTEMPTS YOU HAVE SCORE MINIMUN 3 TO ENTER INTO LEVEL 2---->");
   
        int attempts=0;
        int score=0;
        if(attempts<=5){
            for(int i=1;i<=5;i++){
                 int n=r.nextInt(50);
 System.out.println(n);
                 System.out.println("<----Enter Your Guessed Number from 1 between 50---->");
                 int GuessingNum=sc.nextInt();
                 if(GuessingNum==n){
                     System.out.println("<----You Guessed right num---->");
                     attempts++;
                     score++;
                 }
                else if(GuessingNum>n){
                     System.out.println("<----Guessed num is higher than generated num---->");
                     attempts++;
                 }
                 else if(GuessingNum<n){
                     System.out.println("<----Guessed num is lower than generated num---->");
                     attempts++;
                     
                 }
                 else{
                     System.out.println("<---YOU entered number out of range--->");
                 }
            }
            System.out.println("your score is "+score);
            System.out.println("And you had completed "+ attempts+" attempts");
            System.out.println("YAHOO YOU CONQURERED THIS GAME AND COMPLETED ALL LEVELS OF THE GAME");
        }
      
    }
    public static void main(String[] args){
        
             System.out.println(".........WELCOME TO NUMBER GUESSING GAME ............");
              System.out.println("............ALL THE BEST PLAY WELL....... ");
             
       
        int leveltwo=level1();
        if(leveltwo>=3){
            System.out.println("CONGRATS YOU ENTERED IN LEVEL 2");
           int levelthree= level2();
           if(levelthree>=3){
               System.out.println("CONGRATS YOU ENTERED IN LEVEL 3");
                 System.out.println("press 1 to enter into level 3");
                   System.out.println("press 2 to exit the game");
                   int a=sc.nextInt();
                   if(a==1){
                       level3();
                   }
                   else{
                       System.out.print("Thankyou! Have a Nice Day");
                   }
           }else{
 System.out.println("THE GAME HAS ENDED THANKYOU FOR PLAYING");
}
        }
        else{
            System.out.println("Better Luck Next Time");
        }
     
    }
}
