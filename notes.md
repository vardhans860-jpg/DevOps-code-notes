# devops code notes
# conditional statements
#sai
#1.if ;
   a=10
   b=20
   if[[$a -ge $b]]
   then
   echo "a is bigger"
   fi
#2. if else;
   c=30
   d=40
   if [[ $c -ge $d ]]
   then
   echo " c is bigger "
   else
   echo " d is bigger "
   fi
 #3.if elif
   e=22
   f=90
   g=0
   if [[ $e -ge $f && $e -ge $g ]]
   then
   echo " e is bigger "
   elif [[ $f -ge $g && $f -ge $e ]]
   then
   echo " f is bigger "
   else
   echo " g is bigger "
   fi
#4; case
   echo " enter a number : "
   read num
   case $num in
    1) echo "sunday"
    ;;
    2) echo "monday"
    ;;
    3) echo "tuesday"
    ;;
    4) echo "wednesday"
    ;;
    5) echo "thursday"
    ;;
    6) echo "friday"
    ;;
    7) echo "saturday"
    ;;
    *) echo "invalid"
    ;;
       esac
#loop statements
1.for loop;
    for i in 1 2 3 4 5 6
    do
    echo " numbers; $i "
    done 
         (or)
    for i in {1..10}
    do
    echo $i
    done
    #for even numbers
    for i in {0..10..2}
    do
    echo $i
    done
2.while loop;
    i=10
    while[[$i -ge 0]]
    do
    echo $i
    ((i=i+1))
    done
3.until loop;
    i=1
    until[[$i -eq 11]]
    do
    echo $i
    ((i=i+1))
    done
  
   
