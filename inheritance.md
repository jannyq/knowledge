## Inheritance

### Inheritance in C# #
In inheritance, the derived class inherits all the members (fields, methods) of the base class, but it cannot inherit the constructor of the class class because constructors are not member of a class. Instead of inheriting constructors by the derived class, it is onlu allowed to invoke the constructor of a base class.

When both the base class and the derived class have constructors, both the constructors needs to be executed. To overcome this situation, C# provide a keyword **base**. Using this, the derived class can call the base class constructor.

Code examples:
```
class Tank {
  private int Radius;
  private int Height;

  public Tank(int r, int h) {
    Radius = r;
    Height = h;
  }
}

class AreaOfTank : Tank {
  private string Color;

  public Tank(int c, int r, int h) : base(int r, int h) {
    Color = c;
  }
}
```

The AreaOfTank calls base constructor, so there is no need for AreaOfTank to initialize the values that the base constructor initializes. Note: The base constructor gets called first.
