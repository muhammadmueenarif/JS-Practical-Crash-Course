lec 01. variables 

var for variables and then assign value. 
  var name= "ali";
        var age = "25";
        document.write("Name:" + name +"</br>");
        document.write("Age:" + age);


lec 02. Arrays
program of bubble sort. 

     var arr= new Array (7,2,8,1,3,4);
        var i,j,temp;

        document.write("<br/> <br/> Before Sort...<br/>");
        for (i = 0; i < 6; i++) {
            document.write(arr[i] + "<br/>");
        }

        for (i=0; i<6; i++) {
            for ( j= 0;  j<5; j++) {
                if(arr[j] > arr[j+1]) {

        //below 3 lines to swap value of 0 and 1 index
                    temp= arr[j];
                    arr[j]=arr[j+1];
                    arr[j+1]=temp;
                }   
            }
        }

          document.write("<br/> <br/> After Sort...<br/>");
        for (i = 0; i < 6; i++) {
            document.write(arr[i] + "<br/>");
        }

we assigned value to array. and print each value before sort using for loop. 
then algorithm of bubble sort. 


lec 03. JS Operators.
+, -, *, /, % operators. 

    var num1=40;
        var num2=10;
        document.write(num1 + num2);
        document.write("<br/>");
        document.write(num1 - num2);
        document.write("<br/>");
        document.write(num1 * num2);
        document.write("<br/>");
        document.write(num1 / num2);
        document.write("<br/>");
        document.write(num1 % num2);
        document.write("<br/>");

num1+=5; this means num1=num1+5; so num1 is 40. it will become 40+5= 45. 
var result= (num1 +num2) *5;
document.write(result);

++ for increment and -- for decrement. pre increment and post increment operators. 
== for comparison operator, if (num1==num2). 
!= for not equal to. 
> greater than. < less than. 
>=. <=.

ternary operator. 
var id= prompt("enter user id", "user id");
var pas= prompt ("enter password", "password");

var message= (id=="John" && pas=="1234") ? "welcome" : "invalid user";
alert(message);
//This will show welcome if id is john and pas is 1234. else it will say invalid user. 


Lec 04. Functions 
 
 function sayHello() {
        document.write("Hello there");
    }

    <body>
        <p>Click the following button</p>
        <form>
            <input type="button" onclick="sayHello()" value="sayHello">
        </form>
    </body>

// now we will pass parameters in function.

 <script language="javascript" type="text/javascript">
    function sayHello(name, age) {
        document.write(name + " is" + age +" years old");
    }
    </script>


  <p>Click the following button</p>
    <form>
        <input name="t1" placeholder="Enter Name"> <br>
        <input name="t2" placeholder="Enter Age"> <br>
        <input type="button" onclick="sayHello(t1.value, t2.value)" value="sayHello">
    </form>

make sure that the parameters are passed and accessed in the same order otherwise error occurs. 

// we can make a condition that function will not execute when no value is passed. so that is
we will simply use the following code. 
  <script language="javascript" type="text/javascript">
    function sayHello(name, age) {
        if(name =="" || age=="")
        return;
        document.write(name + " is" + age +" years old");
    }
    </script>


Lec 05. JS Events 
mouse over, mouseout, load. 
<body onload="Load()">

    <img name="img1" onmouseover="MouseOver()" onmouseout="MouseOut()">
</body>

   function Load() {
            document.images["img1"].src= "yellow.png";
        }

        function MouseOver() {
            document.images["img1"].src= "blackpink.png";
        }

        function MouseOut() {
            document.images["img1"].src = "blackyellow.png";
        }

    </script>

