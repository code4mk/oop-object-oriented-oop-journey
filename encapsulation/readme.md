# Encapsulation

Encapsulation is a process of wraping/combine/bind properties and methods (behavior) in a single unit or single container.

![https://www.sitesbay.com/cpp/images/encapsulation-in-cpp.png](https://www.sitesbay.com/cpp/images/encapsulation-in-cpp.png)

All state are private , cannot change  state. Only can change with public function.

# key points of encapsulation.

* Information hiding
* Hide internal states and behavior from external world
* Protect the modification of state

# Example of encapsulation (php)

```php
class BankAccount {
  private $balance;
  
  public function __construct($initialBalance) {
    $this->balance = $initialBalance;
  }
  
  public function deposit($amount) {
    $this->balance += $amount;
  }
  
  public function withdraw($amount) {
    if ($this->balance >= $amount) {
      $this->balance -= $amount;
    } else {
      throw new Exception("Insufficient funds");
    }
  }
  
  public function getBalance() {
    return $this->balance;
  }
}

$bankAccount = new BankAccount(1000);

// Make a deposit
$bankAccount->deposit(500);

// Make a withdrawal
try {
  $bankAccount->withdraw(2000);
} catch (Exception $e) {
  echo $e->getMessage(); // Output: Insufficient funds
}

echo $bankAccount->getBalance(); // Output: 1500
```

# Difference between encapsulation and abstraction

* https://stackoverflow.com/questions/15176356/difference-between-encapsulation-and-abstraction

# Resources

* https://www.sitesbay.com/cpp/cpp-encapsulation
* https://www.freecodecamp.org/news/object-oriented-programming-concepts-21bb035f7260/
* https://www.softwaretestingmaterial.com/encapsulation-in-java/
