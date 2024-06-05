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



