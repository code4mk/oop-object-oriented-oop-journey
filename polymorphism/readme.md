# Polimorphism

* Poly means many and morphism means forms.

## interface

* Interface is blueprint of class and abstract method that means only have method thare have no implementation.

* each method will be public
* method have no implementation but implemented class all methods has implementation
* don't have constructor method

## overriding

* Parent have a method and same method have the child class.that time override the parent method.

```php
class Employee
{
  public function salary()
  {
    return 20000;
  }
}

class SoftwareEngineer
{
  public function salary()
  {
    return 35000;
  }

  public function details()
  {
    echo "Software engineer salary = " . $this->salary();
  }
}

$softwareEngineer = new SoftwareEngineer();
$softwareEngineer->details()
```

## overloading

# resources

* https://www.sitesbay.com/cpp/cpp-polymorphism
* https://phpenthusiast.com/object-oriented-php-tutorials/polymorphism-in-php
