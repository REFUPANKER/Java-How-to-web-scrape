### Java-How-to-web-scrape
---
#### Gets html of page 
---
```java
import java.util.Scanner;
import java.net.URL;
(...)
public static String getHtml (URL uri)
{
try{
String result="";
Scanner sc1=new Scanner(uri.openStream());
   while(sc1.hasNext())
   {
    result+=sc1.nextLine();
    // if result looks like weird , try this ;
    // result+=sc1.nextLine()+"\n";
   }
return result;
}catch(Exception e){
   
   }

}
(...)
```
---
