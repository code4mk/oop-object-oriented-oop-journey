# Inheritance

Inheritance is one of the main pillar of OOP.Child extends Parent class.

# SuperClass | SubClass

* SuperClass: SuperClass (Parent,Base class) which inherited with another class and that class access parent class attributes and methods.

* SubClass: SubClass (child,derived class) which inherit  another class/classess.

```php
// Super class
class Info
{
  private $name = "kamal";

  public function getName()
  {
    return $this->name;
  }
}

// Subclass
class User extends Info
{
  //
}
$user = new User();
$user->getName();
```

# Inheritance type

* single
* multi level
* hierarchical
* hybrid
