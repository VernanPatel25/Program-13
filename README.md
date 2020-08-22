class Calculator1
{
    int ans;
    void add(int a,int b)
    {
        ans=a+b;
        System.out.println(ans);
    }
    void sub(int a,int b)
    {
        ans=a-b;
        System.out.println(ans);
    }
    void mul(int a,int b)
    {
        ans=a*b;
        System.out.println(ans);
    }
    void div(int a,int b)
    {
        ans=a/b;
        System.out.println(ans);
    }
    void calc(int a, int b,char ch)
    {
        switch(ch)
        {
            case '+':
            add(a,b);
            break;
            case '-':
            sub(a,b);
            break;
            case '*':
            mul(a,b);
            break;
            case '/':
            div(a,b);
            break;
            default:
            System.out.println("Please enter +,-,* or / only");
        }
    }
    public static void main(int a, int b, char ch)
    {
        Calculator1 obj=new Calculator1();
        obj.calc(a,b,ch);
    }
}
