class BankAccount {
    private String owner;
    private double balance;

    BankAccount(String owner, double balance) {
        this.owner = owner;
        this.balance = balance;
    }

    void deposit(double amount) {
        balance += amount;
        System.out.println("Deposited: " + amount);
    }

    void withdraw(double amount) {
        if (amount <= balance) {
            balance -= amount;
            System.out.println("Withdrawn: " + amount);
        } else {
            System.out.println("Insufficient funds!");
        }
    }

    void displayBalance() {
        System.out.println(owner + "'s Balance: " + balance);
    }
}

public class BankSystem {
    public static void main(String[] args) {
        BankAccount acc = new BankAccount("Ragul", 1000);
        acc.displayBalance();
        acc.deposit(500);
        acc.withdraw(300);
        acc.withdraw(1500);
        acc.displayBalance();
    }
}
