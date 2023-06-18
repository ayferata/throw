# throw
public int indexOf(String value, String searchedText) throws BatuxException { 	
if(value == null) { throw new BatuxException("Gelen değer null olamaz!"); 	}
	
return value.indexOf(searchedText);
}

import java.util.Scanner; 
public class HataYakala { 
public static void checkAge(int age) { 
if (age < 18) { 
throw new ArithmeticException("Hatalı Yaş");         }

System.out.println("Yasaktan Muaf !");     }

public static void main(String[] args) { Scanner scan = new Scanner(System.in); 
System.out.print("Yaşınız : "); int a = scan.nextInt(); 
try {             checkAge(a);
} catch (ArithmeticException e) {             System.out.println(e.getMessage());
        }

    }
}
