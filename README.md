# ksRECURSION:
When a function calls itself until a specified condition is met.

When there are numerous function calls are waiting due to recursion it is called as Stalk overflow.

Program:
 void print(){
cout << 1 << endl;
print();
}
int main(){
……
print();
return 0;
}          
o/p
1
1
.
.
The specified condition which we have to stop is called the base condition or case. 

Program:
cnt=0
f()
{
if(cnt==3)
return;      (when returns comes in a function it means that function is terminated)
print(cnt)     (value of count is 0)
cnt++
f()            (This function awaits in the memory)
}
main()
{
}
f();
o/p
0
1
2

Recursion Tree
       f()
      f()
    f()
  f()

  PRINT NAME N TIMES USING RECURSION(Time complexity = o(n) )
  void f(i,n)
  {
  if(i>3)
  return;
  print("kavya");
  f(i+1,n);                    o/p       kavya 
  }                                      kavya
  main(){                                kavya
  f(1,n);                                        
PRINT  1-N                           REVERSE ORDER(PRINT N-1)
f(i,N){                              f(i,N){
if(i>N)                              if(i<1)
return;                              return; 
print(i)                             print(i)
f(i+1,N)                             f(i-1,N);
}                                    }
main()                               main()
{                                    {
input(N)                             input(N)
f(1,N)}                              f(N,N)

PRINT LINEARLY FROM 1 TO N(BUT BY BACKTRACK)
f(i,N)
{
if(i<1)
return;
f(i-1,N)
print (i);
}
main(){                           O/P
input(n)                          1
f(N,N);                           2
                                  3

