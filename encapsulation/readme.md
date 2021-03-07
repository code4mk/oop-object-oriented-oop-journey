# Encapsulation
Encapsulation is a process of wraping/combine/bind properties and methods (behavior) in a single unit or single container.

![https://www.sitesbay.com/cpp/images/encapsulation-in-cpp.png](https://www.sitesbay.com/cpp/images/encapsulation-in-cpp.png)

all state is private , cannot change the state. Only can change with public function.

~ Encapsulation or information hiding

~ Hide internal states and values inside a class, (safe the modification of state)

```php
class Cat
{
  private hungry;

  public function feedNow()
  {
    $this->hungry = 'feed';
  }
}
```

# encapsulation vs abstraction

* https://stackoverflow.com/questions/15176356/difference-between-encapsulation-and-abstraction

# resources

* https://www.sitesbay.com/cpp/cpp-encapsulation
* https://www.freecodecamp.org/news/object-oriented-programming-concepts-21bb035f7260/
* https://www.softwaretestingmaterial.com/encapsulation-in-java/
