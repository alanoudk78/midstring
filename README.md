# midstring


package middstring;

public class MiddString {

   
    public static void main(String[] args) {
       String a="Alanoud";
       System.out.println(Midd(a));
    }
    static int Midd(String a){
        int length1=a.charAt(a.length()/2);
        int length2=(a.charAt(a.length()/2))&((a.charAt(a.length()/2))-1);
        if(a.length()==0)
            return 0;
    if(a.length()%2==1)
        return length1;
    if(a.length()%2==0)
        return length2;
     return Midd(a);
}
}
