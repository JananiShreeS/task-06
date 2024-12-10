# task-06 class
package attributes;

public class ClassPerson {
private String name;
private int age;

	public ClassPerson(String name,int age) {
		this.name=name;
		this.age=age;
	}
public String getname() {
	return name;
}
	
public int getage() {
	return age;
}
public static void main(String[] args)
{
		ClassPerson ClassPerson=new ClassPerson("alice",40);
		
	
System.out.println("Name:" + ClassPerson.getname());
System.out.println("age:" + ClassPerson.getage());
}
}


2.Employee details
package attributes;

public class Employee {
	private int Id;
	private String Firstname;
	private String Lastname;
	private int Salary;
	
public Employee(int Id,String Firstname,String Lastname,int Salary) {
	this.Id=Id;
	this.Firstname=Firstname;
	this.Lastname=Lastname;
	this.Salary=Salary;
}
public int getId()
{ 
	return Id;
	}
public String getFirstname()
{
	return Firstname;
}
public String getLastname() {
	return Lastname;
}
public int getSalary()
{
	return Salary;
}
public int setSalary(int Salary) {
	return this.Salary=Salary;
	}
public int getannualSalary(int Salary)
{
	return this.Salary+=Salary*(Salary*12);
}

{
	System.out.println("annual Salary of this id is:");
}
public void raiseSalary(int percent)
{
	if (percent>0)
	{
		Salary+=Salary*(percent/100);
	}
	else
	{
		System.out.println("Percentage must be positive!");
		}
	
	public static void main (String[]args)
	{
		Employee emp= new Employee(1,"ann","alex",25000);
	System.out.println Employee("Id:"= +getId(),"Firstname:"= +getFirstname(),"Lastname:"= +getlastname(),"Salary:"= +getSalary());
		}
		{
		
		System.out.println("before raise:" +Salary);
	emp.getSalary(20);
		}
		System.out.println("after raise of :" +Salary);
	}
}


3.Circle
package constructor;

public class Circle {
	private static final String CircumferenceCircle = null;
	private double radius;
	public Circle()
	{
		this.radius=1.0;
		}
		public Circle (double radius)
		{
			this.radius=radius;
			
		}
		public double getradius()
		{
			return radius;
		}
		public void setradius(double radius)
		{
			this.radius=radius;
			
		}
		public double getCircumference()
		{
			return 2*Math.PI*radius;
		}
	public static void main(String[] args)
	{
Circle defaultCircle = new Circle();
System.out.println("Default Circle:" +defaultCircle);
Circle customCircle =new Circle(5.5);
customCircle.setradius(10.0);
System.out.println("Updated Custom Circle:" +CircumferenceCircle);
	}
}

4.Account

package attributes;

public class Account {
	private String accountnum;
	private double balance;
	public Account() 
	{
	
		this.accountnum="UNKNOWN";
		this.balance=0.0;
	}
	public Account(String accountnum,double balance)
	{
		this.accountnum=accountnum;
		this.balance=balance;
	}
	
		public void deposit(double amount)
		{
			if(amount>0)
			{
				balance += amount;
				System.out.println("Successfully deposited$:" +amount);
			}
			else
			{
				System.out.println("Deposit amount must be positive:" );
			}
	}
	public void withdraw(double amount)
	{
		if(amount>0)
		{
			if(amount<0)
			{
				balance-=amount;
				System.out.println("Successfully withdraw:" +amount);
			}
			else
			{
				System.out.println("insufficient balance:" +balance);
			}
			{
				System.out.println("withdrawn amount must be positive:" );
			}
		}
	}
	public double checkbalance()
	{
		return balance;
		
	}
	 public void displayAccountDetails() 
	 {
	        System.out.println("Account Number: " + accountnum);
	        System.out.println("Balance:"  + balance);
        }
	 public static void main(String[] args)
	 {
		
		 Account account1 = new Account();
	        System.out.println("Account 1 Details (Default):");
	        account1.displayAccountDetails();
	        
	        System.out.println("\nDepositing $500 into Account 1...");
	        account1.deposit(500);
	        account1.displayAccountDetails();
	        
	        System.out.println("\nWithdrawing $200 from Account 1...");
	        account1.withdraw(200);
	        account1.displayAccountDetails();
	        
	        Account account2 = new Account("123456789", 1000.0);
	        System.out.println("\nAccount 2 Details:");
	        account2.displayAccountDetails();
	        
	        System.out.println("\nDepositing $300 into Account 2...");
	        account2.deposit(300);
	        account2.displayAccountDetails();
	        
	        System.out.println("\nWithdrawing $1500 from Account 2...");
	        account2.withdraw(1500);
	        account2.displayAccountDetails();
	}

}
