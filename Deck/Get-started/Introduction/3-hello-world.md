##

```
using System;

class Hello
{
    static void Main()
    {
        Console.WriteLine("Hello, World");
    }
}
```

The "Hello, World" program starts with a `using` directive that references the `System` `_____`. `_____` provide a hierarchical means of organizing C# programs and libraries. `_____` contain types and other `_____` — for example, the `System` `_____` contains a number of types, such as the `Console` class referenced in the program, and a number of other `_____`, such as `IO` and `Collections`. A `using` directive that references a given `_____` enables unqualified use of the types that are members of that `_____`. Because of the `using` directive, the program can use `Console.WriteLine` as shorthand for `System.Console.WriteLine`.

%

The "Hello, World" program starts with a `using` directive that references the `System` **namespace**. **Namespaces** provide a hierarchical means of organizing C# programs and libraries. **Namespaces** contain types and other **namespaces** — for example, the `System` **namespace** contains a number of types, such as the `Console` class referenced in the program, and a number of other **namespaces**, such as `IO` and `Collections`. A `using` directive that references a given **namespace** enables unqualified use of the types that are members of that **namespace**. Because of the `using` directive, the program can use `Console.WriteLine` as shorthand for `System.Console.WriteLine`.

##

```
using System;

class Hello
{
    static void Main()
    {
        Console.WriteLine("Hello, World");
    }
}
```

The `Hello` class declared by the "Hello, World" program has a single member, the `_____` named `Main`. The `Main` `_____` is declared with the `static` modifier. While instance `_____` can reference a particular enclosing object instance using the keyword `this`, static `_____` operate without reference to a particular object. By convention, a static `_____` named `Main` serves as the entry point of a C# program.

%

The `Hello` class declared by the "Hello, World" program has a single member, the **method** named `Main`. The `Main` **method** is declared with the `static` modifier. While instance **methods** can reference a particular enclosing object instance using the keyword `this`, static **methods** operate without reference to a particular object. By convention, a static **method** named `Main` serves as the entry point of a C# program.

##

```
using System;

class Hello
{
    static void Main()
    {
        Console.WriteLine("Hello, World");
    }
}
```

The output of the program is produced by the `WriteLine` method of the `Console` `_____` in the `System` namespace. This `_____` is provided by the standard `_____` libraries, which, by default, are automatically referenced by the compiler.

%

The output of the program is produced by the `WriteLine` method of the `Console` **class** in the `System` namespace. This **class** is provided by the standard **class** libraries, which, by default, are automatically referenced by the compiler.
