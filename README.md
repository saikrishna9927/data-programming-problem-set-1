# data-programming-problem-set-1

Question 1 C# 
What data type is each of the following? 5 5.0 5 > 1 '5' 5 * 2 '5' * 2 '5' + '2' 5 / 2 5 % 2 {5, 2, 1} 5 == 3 Pi (the number)
SOL:
5 5.0 5 > 1 '5' 5 * 2 '5' * 2 '5' + '2' 5 / 2 5 % 2 {5, 2, 1} 5 == 3 Pi (the number)
SOL:
5-int
5.0-int/float
5>1-true-bool
‘5’-int
5*2-10-int
‘5’*2 -
‘5’+’2’-int
5/2->2.5-float
5%2->1-int
{5,2,1}-int
5==3-false-bool	
Pi-float


Question 2 C# Write (and evaluate) C# expressions that answer these questions:
 a. How many letters are there in 'Supercalifragilisticexpialidocious'?
 b. Does 'Supercalifragilisticexpialidocious' contain 'ice' as a substring?
c. Which of the following words is the longest: Supercalifragilisticexpialidocious, Honorificabilitudinitatibus, or Bababadalgharaghtakamminarronnkonn? 
d. Which composer comes first in the dictionary: 'Berlioz', 'Borodin', 'Brian', 'Bartok', 'Bellini', 'Buxtehude', 'Bernstein'. Which one comes last?
SOL:
public class CountCharacter

{
public static void Main()
{
String string1 = “Supercalifragilisticexpialidocious”;
int count = 0;

for(int i=0;i<string1.Length;i++)
{
If(string1[i]!=’ ‘)
count++;
}
Console.WriteLine(“Total number of characters in a string:”+count);
}






Question 4 C# 
Write a program in C# Sharp to separate odd and even integers in separate arrays. Go to the editor 
Test Data : Input the number of elements to be stored in the array :
5 Input 5 elements in the array :
 element - 0 : 25 element - 1 : 47 element - 2 : 42 element - 3 : 56 element - 4 : 32
 Expected Output: The Even elements are: 42 56 32 The Odd elements are :25 47
SOL:
#include<stdio.h>
void display(int a[], int size);
int main(){
   int size, i, a[10], even[20], odd[20];
   int Ecount = 0, Ocount = 0;
   printf("enter size of array :\n");
   scanf("%d", &size);
   printf("enter array elements:\n");
   for(i = 0; i < size; i++){
      scanf("%d", &a[i]);
   }
   for(i = 0; i < size; i ++){
      if(a[i] % 2 == 0){
         even[Ecount] = a[i]; using System;
 
class GFG {
     
    static bool isVowel(char c)
    {
        return (c == 'A' || c == 'E' ||
                c == 'I' || c == 'O' ||
                c == 'U' || c == 'a' ||
                c == 'e' || c == 'i' ||
                c == 'o' || c == 'u');
    }
     
    static string pigLatin(string s)
    {
     
        // the index of the first
        // vowel is stored.
        int len = s.Length;
        int index = -1;
        for (int i = 0; i < len; i++)
         Ecount++;
      }
      else{
         odd[Ocount] = a[i];
         Ocount++;
      }
   }
   printf("no: of elements comes under even are = %d \n", Ecount);
   printf("The elements that are present in an even array is: ");
   display(even, Ecount);
   printf("no: of elements comes under odd are = %d \n", Ocount);
   printf("The elements that are present in an odd array is : ");
   display(odd, Ocount);
   return 0;
}
void display(int a[], int size){
   int i;
   for(i = 0; i < size; i++){ using System;
 
class GFG {
     
    static bool isVowel(char c)
    {
        return (c == 'A' || c == 'E' ||
                c == 'I' || c == 'O' ||
                c == 'U' || c == 'a' ||
                c == 'e' || c == 'i' ||
                c == 'o' || c == 'u');
    }
     
    static string pigLatin(string s)
    {
     
        // the index of the first
        // vowel is stored.
        int len = s.Length;
        int index = -1;
        for (int i = 0; i < len; i++)
      printf("%d \t ", a[i]);
   }
   printf("\n");
}
Output
When the above program is executed, it produces the following result −
enter size of array:
5
enter array elements:
25
47
42
56
32
no: of elements comes under even are = 3.
The elements that are present in an even array is: 42 56 32
no: of elements comes under odd are = 2
The elements that are present in an odd array is : 25 47


Question 5 C# 
a.Write a function inside(x,y,x1,y1,x2,y2) that returns True or False depending on whether the point (x,y) lies in the rectangle with lower left corner (x1,y1) and upper right corner (x2,y2). >>> inside(1,1,0,0,2,3) True >>> inside(-1,-1,0,0,2,3) 
False
b.Use function inside() from part a. to write an expression that tests whether the point (1,1) lies in both of the following rectangles: one with lower left corner (0.3, 0.5) and upper right corner (1.1, 0.7) and the other with lower left corner (0.5, 0.2) and upper right corner (1.1, 2).


Question 6 
Python 
16. You can turn a word into pig-Latin using the following two rules (simplified): 
• If the word starts with a consonant, move that letter to the end and append 'ay'. For example, 'happy' becomes 'appyhay' and 'pencil' becomes 'encilpay'. 
• If the word starts with a vowel, simply append 'way' to the end of the word. For example, 'enter' becomes 'enterway' and 'other' becomes 'otherway' . For our purposes, there are 5 vowels: a, e, i, o, u (so we count y as a consonant). Write a function pig() that takes a word (i.e., a string) as input and returns its pigLatin form. Your function should still work if the input word contains upper case characters. Your output should always be lower case however. 
>>> pig('happy') 'appyhay' 
>>> pig('Enter') 'enterway'

SOL:
using System;
 
class GFG {
     
    static bool isVowel(char c)
    {
        return (c == 'A' || c == 'E' ||
                c == 'I' || c == 'O' ||
                c == 'U' || c == 'a' ||
                c == 'e' || c == 'i' ||
                c == 'o' || c == 'u');
    }
     
    static string pigLatin(string s)
    {
     
        
        int len = s.Length;
        int index = -1;
        for (int i = 0; i < len; i++)
{
            if (isVowel(s[i]))
            {
                index = i;
                break;
            }
        }
 
    
        
        if (index == -1)
            return "-1";
     
       
        return s.Substring(index) +
               s.Substring(0, index)
                              + "ay";
    }
     
    
    public static void Main()
    {
        string str = pigLatin("happy");
if (str == "-1")
            Console.WriteLine("No vowels"
                     + "found. Pig Latin"
                      + " not possible");
        else
            Console.WriteLine(str);
    }
}

OUTPUT
>>> pig('happy')
 'appyhay'
 >>> pig('Enter')
 'enterway'


Question 7 
Python
 File bloodtype1.txt records blood-types of patients (A, B, AB, O or OO) at a clinic. Write a function bldcount() that reads the file with name name and reports (i.e., prints) how many patients there are in each bloodtype.
 >>> bldcount('bloodtype.txt')
 There are 10 patients of blood type A. 
There is one patient of blood type B. 
There are 10 patients of blood type AB.
 There are 12 patients of blood type O. 
There are no patients of blood type OO.


Question 8 Python 
Write a function curconv() that takes as input: 
1. a currency represented using a string (e.g., 'JPY' for the Japanese Yen or 'EUR' for the Euro) 
2. an amount 
and then converts and returns the amount in US dollars.
 >>> curconv('EUR', 100)
 122.96544 
>>> curconv('JPY', 100) 
1.241401 
The currency rates you will need are stored in file currencies.txt: 
AUD 1.0345157 Australian Dollar 
CHF 1.0237414 Swiss Franc 
CNY 0.1550176 Chinese Yuan
DKK 0.1651442 Danish Krone 
EUR 1.2296544 Euro
 GBP 1.5550989 British Pound
 HKD 0.1270207 Hong Kong Dollar
 INR 0.0177643 Indian Rupee 
JPY 0.01241401 Japanese Yen
 MXN 0.0751848 Mexican Peso
 MYR 0.3145411 Malaysian Ringgit
 NOK 0.1677063 Norwegian Krone
 NZD 0.8003591 New Zealand Dollar
 PHP 0.0233234 Philippine Peso 
SEK 0.148269 Swedish Krona
 SGD 0.788871 Singapore Dollar
 THB 0.0313789 Thai Baht

SOL:
print("Please choose which currency you want to convert:")
print("A – New Zealand Dollar to US Dollar (Exchange Rate: 0.000905)")
print("B – New Zealand Dollar to Euro (Exchange Rate: 0.000807350908)")
print("C – New Zealand Dollar to Japanese Yen (Exchange Rate: 0.0919061643)")
print("D – New Zealand Dollar to Chinese RMB (Exchange Rate: 0.00603703605)")
print("E - Quit ")

A=0
B=0
C=0
D=0

usd = 0.000905
eur = 0.000807350908
yen = 0.0919061643
rmb = 0.00603703605

def main():
    (option, amount) = Input()
    Output(totalamount)

def Input():
    option = eval(input("Enter your option: "))
    amount = eval(input("Enter the amoutn in New Zealand Dollar: "))
    if option == "A":
        totalamount = (amount * usd)
        print (amount +"New Zealand dollar equals to "+totalamount+" USD")
    elif option== "B":
        totalamount = (amount * eur)
        print (amount +"New Zealand Dollar  equals to "+totalamount+" Euro")
    elif option== "C":
        totalamount = (amount * yen)
        print (amount +"New Zealand Dollar equals to "+totalamount+" Yen")
    elif option== "D":
        totalamount = (amount * rmb)
        print (amount +"New Zealand Dollar equals to "+totalamount+" Chinese RMB")
    else:
        quit

Question 9 Python
 Each of the following will cause an exception (an error).
 Identify what type of exception each will cause.
 Trying to add incompatible variables, as in adding 6 + ‘a’ 
Referring to the 12th item of a list that has only 10 items
 Using a value that is out of range for a function’s input, such as calling math.sqrt(-1.0) 
Using an undeclared variable, such as print(x) when x has not been defined 
Trying to open a file that does not exist, such as mistyping the file name or looking in the wrong directory.

SOL:








Question 10 Python
 Encryption is the process of hiding the meaning of a text by substituting letters in the message with other letters, according to some system. If the process is successful, no one but the intended recipient can understand the encrypted message. Cryptanalysis refers to attempts to undo the encryption, even if some details of the encryption are unknown (for example, if an encrypted message has been intercepted). The first step of cryptanalysis is often to build up a table of letter frequencies in the encrypted text. Assume that the string letters is already defined as 'abcdefghijklmnopqrstuvwxyz'. Write a function called frequencies() that takes a string as its only parameter, and returns a list of integers, showing the number of times each character appears in the text. Your function may ignore any characters that are not in letters
. >>> frequencies('The quick red fox got bored and went home.') [1, 1, 1, 3, 5, 1, 1, 2, 1, 0, 1, 0, 1, 2, 4, 0, 1, 2, 0, 2, 1, 0, 1, 1, 0, 0] 
>>> frequencies('apple')
