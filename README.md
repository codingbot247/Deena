# Deena
Just a silly conversational program in Java, made in basic Java. 
import java.io.*;
public class deena
{
public static void main(String args[])throws IOException
{
	int fact=1,n,s=0,y=0,to_day=0,da_te=0,l;
	String a=" ",b,c,d,g,str;
    char t;


System.out.println("Hi there! I am Deena");
System.out.println("what's your name?(only the name please)");
BufferedReader br= new BufferedReader(new InputStreamReader(System.in));
a=br.readLine();
System.out.println("Hello "+a);

System.out.println("so how are you?");


/*need to put something so that deena should not wait for an interrupt
*and after that it should directly jump to ask
*users the date and their date of birth
*/


switch(str=(String)br.readLine())
{
	case "fine":
    case "i am fine":
System.out.println("good to know");
break;

     case "okay":
      case "i am okay":
     System.out.println("that's good");
     break;

     case "good":
     case  "i am good":
     System.out.println("well then let us talk a bit");
     break;

     case "better":
      case "i am better":
     System.out.println("okay nice then!");
     break;
     case "nice":
     case "i am nice":
     System.out.println("as expected, but glad to know");
     break;

    default:
    System.out.println("???what do you mean");

}
try{
c=br.readLine();
}
catch(Exception e)
{
	System.out.println("ummmmmmm.........");
}
System.out.println("What is the date today");
try{
to_day=Integer.parseInt(br.readLine());
}
catch(Exception e)
{
	System.out.println("while entering the date plz dont mention the month and year");
	System.out.println("so tell me the date now");
	l=Integer.parseInt(br.readLine());
}


System.out.println("lets talk about your birthday");
System.out.println("please enter the date of your birth but dont give me the month and year");
da_te=Integer.parseInt(br.readLine());

if(da_te==to_day)
{
	System.out.println("hey dear today is your birthday");
	System.out.println("HAPPY BITHDAY DEAR "+a);
}
else
{
	System.out.println("oh so we have to wait for your birhtday");
}
System.out.flush();


d=br.readLine();


System.out.println("hey! do you want some more  ");
g=br.readLine();


System.out.println("\n So I have a list of things that i can do for you   ");
if(s==y)
{
	System.out.println("1..fibonacci series");
	System.out.println("2..A joke");
	System.out.println("3..check palindrome or not");
	System.out.println("4..about myself");
	System.out.println( "5..five great signs of an intelligent being");
	System.out.println( "6..find factorial of a number");
}
else
{
	System.out.println("what would you like then?");

}

try{
switch( t=(char)System.in.read())
{
	case '1':
int o=1,p=1,r=0;
System.out.print("1 1 ");

do{

r=o+p;
System.out.print(r+"  ");

o=p;
p=r;
}while(r<=50);
break;

case '2': System.out.println("what did an ant say to an Elephant that made him cry?");





System.out.println("that I ate your bananas!!!");
break;

case '3':

int w=0;
int rem,num=w,sum=0;
System.out.print("enter the number to check for palindrome");
int v=Integer.parseInt(br.readLine());
while(num!=0)
{
	rem=num%10;
	num=num/10;
	sum=sum*10+rem;
	System.out.println(""+sum);
}

if(sum==num)
{
	System.out.println("the number is a palindrome number");
}

else
{
	System.out.println("the number is not a palindrome");
}
break;

case '4':
System.out.println("I am a baby digital assistant made to help you do things");
System.out.println("I am yet to develope more and eager to be a part of the Artificial Intelligence world");
break;

case '5':
System.out.println("These are.............");
System.out.println("They are always optimistic");
System.out.println("They think out of the box");
System.out.println("They are never afraid of taking risks");
System.out.println("They work for the good for society and to help make this world a better place");
System.out.println("They work smarter and innovatively");
break;

case '6':

System.out.println("enter the number to find factorial");
n=Integer.parseInt(br.readLine());

do
{
fact=fact*n;
n--;
}

while(n>=1);
System.out.println("factorial is  "+fact);
break;


default:
System.out.println("sorry! at this time i can do only the above mentioned things in the list");
int dem=Integer.parseInt(br.readLine());

}


}
catch(Exception e)
{
	System.out.println("oh no a major error is disturbing me!I have to go sorry :(");
}


}
}
