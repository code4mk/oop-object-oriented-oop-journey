# Polimorphism

Poly means many and morphism means forms.In Polimorphism an object can behave many form based on context.

Polymorphism is achieved by using method overloading and method overriding.

## interface
Interface is blueprint of class and abstract method that means only have method thare have no implementation.

* each method will be public
* Method have no implementation
* Don't have constructor method

# overriding

* orverriding is ability to modification the behavior or implement the expected bahavior on child class . override method which is contain both parent and child class.

```php
class Shape {
    public function draw() {
        return "Drawing a shape.";
    }
}

class Circle extends Shape {
    public function draw() {
        return "Drawing a circle.";
    }
}

$shape = new Shape();
echo $shape->draw(); // Outputs: "Drawing a shape."

$circle = new Circle();
echo $circle->draw(); // Outputs: "Drawing a circle."

```

## overloading
In object-oriented programming, "overloading" refers to the ability to create multiple methods with the same name but with different parameters. This is achieved by providing multiple definitions for the same method name in a class.

* overload method is method inside same class, method name is same but parameters name is different.

```php
class Calculator {
    public function add($a, $b) {
        return $a + $b;
    }

    public function add($a, $b, $c) {
        return $a + $b + $c;
    }
}

$calculator = new Calculator();
echo $calculator->add(1, 2); // Outputs: 3
echo $calculator->add(1, 2, 3); // Outputs: 6
```

In this example, the Calculator class defines two methods with the same name add, but with different parameters. The correct method to be called is determined by the number of arguments that are passed to the method. When we call add with two arguments, it outputs "3", and when we call it with three arguments, it outputs "6".

# resources

* https://www.sitesbay.com/cpp/cpp-polymorphism
* https://phpenthusiast.com/object-oriented-php-tutorials/polymorphism-in-php
