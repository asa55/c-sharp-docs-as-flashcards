##

The key organizational concepts in C# are

- `_____`
- `_____`
- `_____`
- `_____`
- `_____`

%

- programs
- namespaces
- types
- members
- and assemblies

##

`_____` declare types, which contain members and can be organized into namespaces. 

%

**Programs** declare types, which contain members and can be organized into namespaces. 

##

Classes, structs, and interfaces are examples of

%

types

##

Fields, methods, properties, and events are examples of

%

members

##

When C# programs are compiled, they're physically packaged into

%

assemblies

##

Assemblies typically have the file extension `.exe` or `.dll`, depending on whether they implement `_____` or `_____`, respectively.

%

Assemblies typically have the file extension `.exe` or `.dll`, depending on whether they implement **applications** or **libraries**, respectively.

##

Consider an assembly that contains the following code:

```
namespace Acme.Collections;

public class Stack<T>
{
    Entry _top;

    public void Push(T data)
    {
        _top = new Entry(_top, data);
    }

    public T Pop()
    {
        if (_top == null)
        {
            throw new InvalidOperationException();
        }
        T result = _top.Data;
        _top = _top.Next;

        return result;
    }

    class Entry
    {
        public Entry Next { get; set; }
        public T Data { get; set; }

        public Entry(Entry next, T data)
        {
            Next = next;
            Data = data;
        }
    }
}
```

The fully qualified name of this class is `_____`. The class contains several members: a field named `_____`, two methods named `_____` and `_____`, and a nested class named `_____`. The `_____` class further contains three members: a property named `_____`, a property named `_____`, and a constructor. The `_____` is a generic class. It has one type parameter, `_____` that is replaced with a concrete type when it's used.

%

The fully qualified name of this class is `Acme.Collections.Stack`. The class contains several members: a field named `_top`, two methods named `Push` and `Pop`, and a nested class named `Entry`. The `Entry` class further contains three members: a property named `Next`, a property named `Data`, and a constructor. The `Stack` is a generic class. It has one type parameter, `T` that is replaced with a concrete type when it's used.

##

Consider an assembly that contains the following code:

```
namespace Acme.Collections;

public class Stack<T>
{
    Entry _top;

    public void Push(T data)
    {
        _top = new Entry(_top, data);
    }

    public T Pop()
    {
        if (_top == null)
        {
            throw new InvalidOperationException();
        }
        T result = _top.Data;
        _top = _top.Next;

        return result;
    }

    class Entry
    {
        public Entry Next { get; set; }
        public T Data { get; set; }

        public Entry(Entry next, T data)
        {
            Next = next;
            Data = data;
        }
    }
}
```

A `_____` is a "first in - last out" (FILO) collection. New elements are added to the top of the `_____`. When an element is removed, it's removed from the top of the `_____`. The previous example declares the `_____` type that defines the storage and behavior for a `_____`. You can declare a variable that refers to an instance of the `_____` type to use that functionality.

%

A **stack** is a "first in - last out" (FILO) collection. New elements are added to the top of the **stack**. When an element is removed, it's removed from the top of the **stack**. The previous example declares the `Stack` type that defines the storage and behavior for a **stack**. You can declare a variable that refers to an instance of the `Stack` type to use that functionality.

##

Assemblies contain executable code in the form of Intermediate Language (IL) instructions, and symbolic information in the form of metadata. Before it's executed, the Just-In-Time (JIT) compiler of .NET Common Language Runtime converts the IL code in an assembly to

%

processor-specific code

##

```
class Example
{
    public static void Main()
    {
        var s = new Acme.Collections.Stack<int>();
        s.Push(1); // stack contains 1
        s.Push(10); // stack contains 1, 10
        s.Push(100); // stack contains 1, 10, 100
        Console.WriteLine(s.Pop()); // stack contains 1, 10
        Console.WriteLine(s.Pop()); // stack contains 1
        Console.WriteLine(s.Pop()); // stack is empty
    }
}
```

Because an assembly is a self-describing unit of functionality containing both code and metadata, there's no need for `#include` directives and header files in C#. The public types and members contained in a particular assembly are made available in a C# program simply by referencing that assembly when compiling the program. For example, the following program uses the `_____` class from the `_____` assembly.

%

Because an assembly is a self-describing unit of functionality containing both code and metadata, there's no need for `#include` directives and header files in C#. The public types and members contained in a particular assembly are made available in a C# program simply by referencing that assembly when compiling the program. For example, the following program uses the `Acme.Collections.Stack` class from the `acme.dll` assembly.

##

C# programs can be stored in several source `_____`. When a C# program is compiled, all of the source `_____` are processed together, and the source `_____` can freely reference each other. Conceptually, it's as if all the source `_____` were concatenated into one large `_____` before being processed. Forward declarations are never needed in C# because, with few exceptions, declaration order is insignificant. C# doesn't limit a source `_____` to declaring only one public type nor does it require the name of the source `_____` to match a type declared in the source `_____`.

%

C# programs can be stored in several source **files**. When a C# program is compiled, all of the source **files** are processed together, and the source **files** can freely reference each other. Conceptually, it's as if all the source **files** were concatenated into one large **file** before being processed. Forward declarations are never needed in C# because, with few exceptions, declaration order is insignificant. C# doesn't limit a source **file** to declaring only one public type nor does it require the name of the source **file** to match a type declared in the source **file**.
