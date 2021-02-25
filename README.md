# ExceptionHandling
Codes of Exception Handling
import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        // put your code here
        Scanner scanner = new Scanner(System.in);
        List<String> list = new ArrayList();
        while (scanner.hasNext()) {
            String input = scanner.next();
            if (!input.equals("0")) {
                list.add(input);
            } else {
                break;
            }
        }
        int[] output = new int[list.size()];
        for (int i = 0; i < list.size(); i++) {

            try {
                System.out.println(Integer.parseInt(list.get(i)) * 10);
            } catch (Exception e) {

                System.out.println("Invalid user input: " + list.get(i));
            }

        }


    }
}//




import java.util.*;

public class Main {
    public static void main (String[] args) {
    Scanner sc = new Scanner(System.in);
    String a;
    while(sc.hasNext()) {
    	
    	a = sc.next();
    
    	if(a.equals("0")) {
    		break;
    	}
    	try {
    		int b = Integer.parseInt(a);
    		System.out.println(b*10);
    	}catch(Exception e) {
    		System.out.println("Invalid user input: "+a);
    	}
    }
    
}
}
