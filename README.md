// Online Java Compiler
// Use this editor to write, compile and run your Java code online

class Main {
    public static void main(String[] args) {
        // String s = "Hello";
        // s = s + "world";
        // System.out.println(s);
        // System.out.print("String is immutable in java that can not been change ");
        // System.out.println();
        // String Name = new String("vishal");
        // System.out.print(Name);
        
        // String s = "Hello world";
        // System.out.println("length of String is " + s.length());
        // System.out.println(s.charAt(0));
        // System.out.println(s.substring(0,5));
        
        // String a = "Hii";
        // String b = "Hiii";
        // System.out.println(a.equals(b)); // give true or false
        
        // System.out.println(a.compareTo(b)); // give 0 or -1
        
        // System.out.println(s.contains("wo")); // give true or false
        
        // String c = s.toUpperCase();
        // String d = s.toLowerCase();
        // System.out.print(c);
        // System.out.println();
        // System.out.print(d);
        
        String name = "vishal rajput";
        
        // String p1 = name.substring(0,1);
        // String p2 = name.substring(0,6).toUpperCase();
        // String p3 = name.substring(6);
        
        // String result = p2 + p3;
        // System.out.print(result); 
        //output : VISHAL rajput
        
        for(int i = 0; i < name.length(); i++) {
            // System.out.print(name.charAt(i));
        }
        
        //String revers
        String Name = "isha rajput";
        String rev = "";
        for(int i = Name.length()-1; i >= 0; i--) {
            rev += Name.charAt(i);
        }
        // System.out.print(rev);
        
        //StringBuilder 
        /*
        StringBuilder sb = new  StringBuilder("Hello");
        sb.append(" world");
        System.out.print(sb);
        
        System.out.println();
        
        sb.insert(5, " java");
        System.out.print(sb);
        
        System.out.println();
        
        sb.delete(6,10);
        System.out.print(sb);
        
        System.out.println();
        
        sb.reverse();
        System.out.print(sb);
        
        System.out.println();
        
        System.out.print(sb.charAt(1));
        
        System.out.println();
        
       sb.setCharAt(0, 'V');
       System.out.print(sb);
       
       System.out.println();
       
       System.out.println(sb.length());
       
       sb.reverse();
       String str = sb.toString();
       System.out.print(str);
       */
       
      StringBuilder sb = new StringBuilder();
      for(int i = 0; i < 5; i++) {
          sb.append(i);
      }
      System.out.print(sb.toString());
      
      System.out.println();
      
      String s = "hello";
      String Rev = new StringBuilder(s).reverse().toString();
      System.out.print(Rev);
      
      System.out.println();
      
      String sv = "madam";
      String r1 = new StringBuilder(sv).reverse().toString();
      
     if(sv.equals(r1)) {
         System.out.print("Palidrome");
     }
     else {
         System.out.print("not palidrome");
     }
       
        
        
        
        
        
    }
}