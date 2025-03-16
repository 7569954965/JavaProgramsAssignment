# JavaProgramsAssignment

# 1.String Manipulation AnagramCheck
import java.util.Arrays;

public class StringAnagramCheck {

	public static void main(String[] args) {	
		String str1="gum";
		String str2="mugh";
		System.out.println(anagrams(str1,str2));	
	}
	static boolean anagrams(String str1, String str2) {	
		char[] str1Array=str1.toCharArray();
		char[] str2Array=str2.toCharArray();
		Arrays.sort(str1Array);
		Arrays.sort(str2Array);
		return Arrays.equals(str1Array, str2Array);
		
	}
}

output->false

#2.OOPS -Employee Management System.
import java.util.ArrayList;

public class Employee {
	
	int id;
	String name;
	int salary;
	void displayDetails(int id,String name,int salary) {
		this.id=id;
		this.name=name;
		this.salary=salary;
  
//		System.out.println(id +" " + name + " " + salary);

	}
	
	public static void main(String args[]) {
		
		Employee obj1= new Employee();
		obj1.displayDetails(1, "Pavan", 100000);
		Employee obj2= new Employee();
		obj2.displayDetails(2, "Kumar", 200000);
		Employee obj3= new Employee();
		obj3.displayDetails(3, "Rao", 300000);
		Employee obj4= new Employee();
		obj4.displayDetails(4, "Naruto", 400000);
		Employee obj5= new Employee();
		obj5.displayDetails(5, "Hinata", 500000);
		
		
		ArrayList<Employee> list= new ArrayList<>(); 
		list.add(obj1);
		list.add(obj2);
		list.add(obj3);
		list.add(obj4);
		list.add(obj5);
//		System.out.println(list.size());

		for(int i=0;i<list.size();i++) {
			
			System.out.println(list.get(i).id + " " + list.get(i).name + " " + list.get(i).salary);
			
		}
		
		
		
	}

}


