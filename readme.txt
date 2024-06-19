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