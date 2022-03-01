# Angelica-Gaton_BSIS-1A-_Computer-Programming-II_-Activity
class MainCountingDuplicateCharacters{  

  public static void main(String args[]){  

     String string1 = "Good Friday";  

        int count;  

          

        char string[] = string1.toCharArray();  

          

        System.out.println("Duplicate characters in a given string: ");   

        for(int o = 0; o <string.length; o++) {  

            count = 1;  

            for(int c = o+1; c <string.length; c++) {  

                if(string[o] == string[c] && string[c] != ' ') {  

                    count++;    

                    string[c] = '0';  

                }  

            }   

            if(count > 1 && string[o] != '0')  

                System.out.println(string[o]);  

        }  

    }  

}  

+ javac -cp . Main.java

+ java -cp . Main

Duplicate characters in a given string: 

o

d






class MainFindingTheFirstNonrepeatedCharacter{  

 public static void main(String args[]){  

     

        String inputStr ="programming";

        for(char i :inputStr.toCharArray()){

        if ( inputStr.indexOf(i) == inputStr.lastIndexOf(i)) {

            System.out.println("First non-repeated character is: "+i);

            break;

        }

    }

}

}
 javac -cp . Main.java

+ java -cp . Main

First non-repeated character is: p

class MainCheckingWhetherAStringContainsOnlyDigit{  

  public static void main(String args[]){  

    String str = "3672815";

    boolean result = str.matches("[0-9]+");

    System.out.println("Original String : " + str);

    System.out.println("Does string contain only Digits? : " + result);

  }

}

 javac -cp . Main.java

+ java -cp . Main

Original String : 3672815

Does string contain only Digits? : true
 
 
 class MainRemovingWhiteSpaceFromAString{  

  public static void main(String args[]){  

      String Str = new String("A humanoid called Titans");

      System.out.print("Return Value :" );

      System.out.println(Str.replaceAll(" ", ""));

   }

}

 
 
