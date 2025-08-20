import java.util.*;
class caesar
{
    public static void main(String[] args) 
    {
        Scanner sc=new Scanner(System.in); 
        int a,i,b;
        String s,d="",f="";
        char ch,c;
        System.out.print("enter string to be encoded");
        s=sc.nextLine();
        System.out.print("enetr the shift length");
        a=sc.nextInt();
        //encoding
        for(i=0;i<s.length();i++)
        {
            ch=s.charAt(i);//extraction of characters
            b=(int)ch;//using of ascii values
            if(b>=65&&b<=90)//For uppercase
            {
                b=b+a;
                if(b>90)//for X,Y,Z
                {
                    b=b-90+64;
                }
                c=(char)b;//coverting back to characters
                d=d+c;//Recollecting the characters
            }
            else if(b>=97&&b<=122)//for lowercase
            {
                b=b+a;
                if(b>122)//for x,y,z
                {
                    b=b-122+96;
                }
                c=(char)b;
                d=d+c;
            }
            else//for characters other than alphabets
                d=d+ch;
        }
        System.out.print("encoded mesage"+d);//encoded character 
        //decoding
        for(i=0;i<d.length();i++)
        {
            ch=d.charAt(i);
            b=(int)ch;
            if(b>=65&&b<=90)
            {
                b=b-a;
                if(b<65)
                {
                    b=91-(65-b);
                }
                c=(char)b;
                f=f+c;
            }
            else if(b>=97&&b<=122)
            {
                b=b-a;
                if(b<97)
                {
                    b=123-(97-b);
                }
                c=(char)b;
                f=f+c;
            }
            else
                f=f+ch;
        }  
        System.out.print("decoded message:"+f);      
    }
  }
}
