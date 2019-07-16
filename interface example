import java.util.Arrays;
import java.util.Comparator;

class Person1 {

	private String name;
	private int age;
  
	public int getAge() {
		return this.age;
	}
  
	public String getName() {
		return this.name;
	}
  
	public Person1(String name,int age) {
		this.name=name;
		this.age=age;
	}
  
	@Override
	public String toString() {
		return "Person [name=" + name + ", age=" + age + "]";
	}

	public int hashCode() {
		return this.age;
	}
  
	public boolean equals(Person1 obj) {
		return(this.getAge() == obj.getAge());
	}
}

class CompareByAge implements Comparator<Person1>{

	@Override
	public int compare(Person1 o1, Person1 o2) {
		return (o1.getAge()-o2.getAge());
	}
	
}

class CompareByName implements Comparator<Person1>{

	@Override
	public int compare(Person1 o1, Person1 o2) {
		return(o1.getName().compareTo(o2.getName()));
	}
	
}
public class TestPerson {

      public static void main(String args[]) {
    	  Person1 persons[]= { new Person1("abc",15),
    			              new Person1("def",95),
    			              new Person1("xyz",42),
    			              new Person1("pqr",26),
    			              new Person1("klm",78)
    	  };
        
    	  Arrays.sort(persons,new CompareByAge());
        
    	  for(Person1 p : persons) {
    		  System.out.println(p.toString());
    	  }
    	  
    	  System.out.println("-----------------------");
    	  
    	  Arrays.sort(persons,new CompareByName());
        
    	  for(Person1 p : persons) {
    		  System.out.println(p.toString());
    	  }
    	  
      }
}
