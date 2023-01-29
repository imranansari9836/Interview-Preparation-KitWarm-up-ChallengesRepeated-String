 public static long repeatedString(String s, long n) {
    // Write your code here
    long count=0;
    for(int i=0;i<s.length();i++)
    {
       if(s.charAt(i)=='a') count++;//2
    }
    long rep=n/s.length();//10/3=3
    count=count*rep;//2*3=6
    long rem=n%s.length();//1
    for(int i=0;i<rem;i++)
    {
        if(s.charAt(i)=='a')count++;//7
    }
    return count;

    }

}
