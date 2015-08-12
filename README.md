# static
#



fun3(int x)       
{
  static int a=3;      //在int = a前加 static ,则变为全局变量,只进行一次初始化
  a+=x;
  return(a);
}
main()
{
  int k=2, m=1, n;
  n=fun3(k);        //a = a+2; 所以a = 5;
  n=fun3(m);       //  a = a + 1 所以 a = 5 + 1 = 6;
  printf("%d ",n);
}
