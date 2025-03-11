class ATM:
    def __init__(self, balance=0):
        self.balance = balance
    
    def check_balance(self):
        print(f"Your current balance is: ${self.balance}")
    
    def deposit(self, amount):
        if amount > 0:
            self.balance += amount
            print(f"Deposited ${amount}. Your new balance is: ${self.balance}")
        else:
            print("Invalid deposit amount.")
    
    def withdraw(self, amount):
        if amount > self.balance:
            print("Insufficient funds.")
        elif amount <= 0:
            print("Invalid withdrawal amount.")
        else:
            self.balance -= amount
            print(f"Withdrawn ${amount}. Your new balance is: ${self.balance}")
    
    def atm_interface(self):
        while True:
            print("\nWelcome to the ATM")
            print("1. Check Balance")
            print("2. Deposit Money")
            print("3. Withdraw Money")
            print("4. Exit")
            
            choice = input("Enter your choice: ")
            
            if choice == '1':
                self.check_balance()
            elif choice == '2':
                amount = float(input("Enter amount to deposit: "))
                self.deposit(amount)
            elif choice == '3':
                amount = float(input("Enter amount to withdraw: "))
                self.withdraw(amount)
            elif choice == '4':
                print("Thank you for using the ATM. Goodbye!")
                break
            else:
                print("Invalid choice. Please select a valid option.")

# Initialize ATM with an initial balance of $1000
if __name__ == "__main__":
    atm = ATM(1000)
    atm.atm_interface()
