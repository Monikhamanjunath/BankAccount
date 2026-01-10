public class BankService {

// Nested class (can be public or private, doesn&#39;t matter for functionality)
static class BankAccount {
private double balance;

public BankAccount(double initialBalance) {
if (initialBalance &lt; 0) {
throw new IllegalArgumentException(&quot;Initial balance cannot be negative&quot;);
}
this.balance = initialBalance;
}

public void deposit(double amount) {
if (amount &lt;= 0) {
throw new IllegalArgumentException(&quot;Deposit must be positive&quot;);
}
balance += amount;
}

public void withdraw(double amount) {
if (amount &lt;= 0 || amount &gt; balance) {
throw new IllegalArgumentException(&quot;Invalid withdrawal&quot;);
}
balance -= amount;
}

public double getBalance() {
return balance;
}
}

// The main entry point
public static void main(String[] args) {
// Create an instance of the BankAccount class
BankAccount acc = new BankAccount(5000);

System.out.println(&quot;Initial Balance: &quot; + acc.getBalance());

// Perform operations
acc.deposit(700);
System.out.println(&quot;Balance after deposit of 500: &quot; + acc.getBalance());

acc.withdraw(100);
System.out.println(&quot;Balance after withdrawal of 300: &quot; + acc.getBalance());

// Print final result
System.out.println(&quot;Final Balance: &quot; + acc.getBalance());
}
}
