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

 javac -cp . Main.java

+ java -cp . Main

Return Value :AhumanoidcalledTitans
 
 
 class MainCheckingwhetherTwoStringsAreAnagram {

  public static void main(String[] args) {

    String str1 = "listen";

    String str2 = "silent";

    

    str1 = str1.toLowerCase();

    str2 = str2.toLowerCase();

    if(str1.length() == str2.length()) {

      char[] charArray1 = str1.toCharArray();

      char[] charArray2 = str2.toCharArray();

      Arrays.sort(charArray1);

      Arrays.sort(charArray2);

      boolean result = Arrays.equals(charArray1, charArray2);

      if(result) {

        System.out.println(str1 + " and " + str2 + " are anagram.");

      }

      else {

        System.out.println(str1 + " and " + str2 + " are not anagram.");

      }

    }

    else {

      System.out.println(str1 + " and " + str2 + " are not anagram.");

    }

  }

}
javac -cp . Main.java

+ java -cp . Main

listen and silent are anagram.


 
