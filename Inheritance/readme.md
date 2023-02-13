# Inheritance
Inheritance is a fundamental concept of OOP, a class can inherit propertis(data) and behavior (method) from a parent class.

# Inheritance example (php)

-> parent class

```php
class Car {
  public $make;
  public $model;
  public $year;
  
  public function getDetails() {
    return "Make: " . $this->make . " Model: " . $this->model . " Year: " . $this->year;
  }
}
```

-> child class 

```php

class SportsCar extends Car {
  public $price = 1200;
  
  public function getPrice() {
    return $this->price;
  }
}

$sportsCar = new SportsCar();
$sportsCar->make = "Porsche";
$sportsCar->model = "911 Turbo";
$sportsCar->year = 2022;

echo $sportsCar->getDetails();
// Output: Make: Porsche Model: 911 Turbo Year: 2022
```

# Difference between super and sub class

* `Super class`: Super class known as parent or base class. It inherited with another class (subclass). 

* `SubClass`: SubClass is known as child class which inherit  another class. Subclass can access properties and method from parent class.

# Inheritance types:
* single
* multi level
* hierarchical
* hybrid
