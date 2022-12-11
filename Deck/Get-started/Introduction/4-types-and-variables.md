##

In C#, a type defines the structure and behavior of any

%

data

##

The declaration of a type may include its members, base type, interfaces it implements, and operations permitted for

%

that type

##

A variable is a label that refers to an instance of a specific

%

type

##

There are two kinds of types in C#:

%

- value types and
- reference types

##

Variables of value types directly contain their

%

data

##

Variables of reference types store references to their

%

data

##

With reference types, it's possible for two variables to reference the same

%

object

##

With reference types, it's possible for operations on one variable to affect the object referenced by the other

%

variable

##

With value types, the variables each have their own copy of the data. Except for `ref` and `out` parameter variables, and it isn't possible for operations on one to affect

%

the other

##

An identifier is a variable

%

name

##

An identifier is a sequence of unicode characters without any 

%

whitespace

##

An identifier may be a C# reserved word, if it's prefixed by

%

`@`

##

Using a reserved word as an identifier can be useful when interacting with other

%

languages

##

C#'s value types are further divided into

- `_____`
- `_____`
- `_____`
- `_____`
- `_____`

%

- simple types
- enum types
- struct types
- nullable value type
- and tuple value types

##

C#'s reference types are further divided into

- `_____`
- `_____`
- `_____`
- `_____`

%

- class types
- interface types
- array types
- and delegate types

##

"Value types" include "Simple types" which include:

- `_____`
- `_____`
- `_____`
- `_____`
- `_____`
- `_____`

%

- Signed integral
- Unsigned integral
- Unicode characters
- IEEE binary floating-point
- High-precision decimal floating-point
- Boolean

##

"Value types" contain "Simple types" which contain "Signed integral", including

- `_____`
- `_____`
- `_____`
- `_____`

%

- `sbyte`
- `short`
- `int`
- `long`

##

"Value types" contain "Simple types" which contain "Unsigned integral", including

- `_____`
- `_____`
- `_____`
- `_____`

%

- `byte`
- `ushort`
- `uint`
- `ulong`

##

"Value types" contain "Simple types" which contain "Unicode characters", including

- `_____`

%

- `char`, which represents a UTF-16 code unit

##

"Value types" contain "Simple types" which contain "IEEE binary floating-point", including

- `_____`
- `_____`

%

- `float`
- `double`

##

"Value types" contain "Simple types" which contain "High-precision decimal floating-point", including

- `_____`

%

- `decimal`

##

"Value types" contain "Simple types" which contain "Boolean", including

- `_____`

%

- `bool`, which represents Boolean values—values that are either `true` or `false`

##

"Value types" include "Enum types" which include:

- `_____`

%

- User-defined types of the form `enum E {...}`. 

##

An `_____` type is a distinct type with named constants. Every `_____` type has an underlying type, which must be one of the eight integral types. The set of values of an `_____` type is the same as the set of values of the underlying type.

%

An **enum** type is a distinct type with named constants. Every **enum** type has an underlying type, which must be one of the eight integral types. The set of values of an **enum** type is the same as the set of values of the underlying type.

##

"Value types" include "Struct types" which include:

- `_____`

%

- User-defined types of the form `struct S {...}`. 

##

"Value types" include "Nullable types" which include:

- `_____`

%

- Extensions of all other value types with a `null` value 

##

"Value types" include "Tuple value types" which include:

- `_____`

%

- User-defined types of the form `(T1, T2, ...)`. 

##

"Reference types" include "Class types" which include:

- `_____`
- `_____`
- `_____`

%

- Ultimate base class of all other types: `object`
- Unicode strings: `string`, which represents a sequence of UTF-16 code units
- User-defined types of the form `class C {...}`

##

"Reference types" include "Interface types" which include:

- `_____`

%

- User-defined types of the form `interface I {...}`

##

"Reference types" include "Array types" which include:

- `_____`

%

- Single-dimensional, multi-dimensional, and jagged. For example: `int[]`, `int[,]`, and `int[][]`

##

"Reference types" include "Delegate types" which include:

- `_____`

%

- User-defined types of the form `delegate int D(...)`

##

C# programs use `_____` to create new types.

%

C# programs use **type declarations** to create new types.

##

A `_____` specifies the name and the members of the new type.

%

A **type declaration** specifies the name and the members of the new type.

##

Six of C#'s categories of types are user-definable:

%

- class types
- struct types
- interface types
- enum types
- delegate types
- and tuple value types

##

You can declare `record` types, either `record struct`, or `record class`. You use records primarily for storing values, with minimal associated behavior. Record types have compiler-synthesized

%

members

##

A class type defines a data structure that contains data members (fields) and function members (methods, properties, and others). Class types support single inheritance and polymorphism, mechanisms whereby derived classes can extend and specialize base classes.

##

A struct type is similar to a class type in that it represents a structure with data members and function members. However, unlike classes, structs are value types and don't typically require heap allocation. Struct types don't support user-specified inheritance, and all struct types implicitly inherit from type object.

##

An interface type defines a contract as a named set of public members. A class or struct that implements an interface must provide implementations of the interface's members. An interface may inherit from multiple base interfaces, and a class or struct may implement multiple interfaces.

##

A delegate type represents references to methods with a particular parameter list and return type. Delegates make it possible to treat methods as entities that can be assigned to variables and passed as parameters. Delegates are analogous to function types provided by functional languages. They're also similar to the concept of function pointers found in some other languages. Unlike function pointers, delegates are object-oriented and type-safe.

##

The class, struct, interface, and delegate types all support `_____`, whereby they can be parameterized with other types.

%

The class, struct, interface, and delegate types all support **generics**, whereby they can be parameterized with other types.

##

C# supports single-dimensional and multi-dimensional arrays of any

%

type

##

Array types don't have to be declared before they can be

%

used

##

Array types are constructed by following a type name with square brackets. For example, `int[]` is a single-dimensional array of `int`, `int[,]` is a two-dimensional array of `int`, and `int[][]` is a single-dimensional array of single-dimensional arrays, also known as a

%

"jagged" array, of int

##

Nullable types don't require a separate definition. For each non-nullable type `T`, there's a corresponding nullable type `T?`, which can hold an additional value, `_____`. For instance, `int?` is a type that can hold any 32-bit integer or the value `_____`, and `string?` is a type that can hold any `string` or the value `_____`.

%

Nullable types don't require a separate definition. For each non-nullable type `T`, there's a corresponding nullable type `T?`, which can hold an additional value, **null**. For instance, `int?` is a type that can hold any 32-bit integer or the value **null**, and `string?` is a type that can hold any `string` or the value **null**.

##

C#'s type system is unified such that a value of any type can be treated as an

%

`object`

##

Every type in C# directly or indirectly derives from the `_____` class type, and `_____` is the ultimate base class of all types. Values of reference types are treated as objects simply by viewing the values as type `_____`. Values of value types are treated as objects by performing boxing and unboxing operations. In the following example, an `int` value is converted to `_____` and back again to `int`.

```
int i = 123;
object o = i;    // Boxing
int j = (int)o;  // Unboxing
```

%

Every type in C# directly or indirectly derives from the `object` class type, and `object` is the ultimate base class of all types. Values of reference types are treated as objects simply by viewing the values as type `object`. Values of value types are treated as objects by performing boxing and unboxing operations. In the following example, an `int` value is converted to `object` and back again to `int`.

##

When a value of a value type is assigned to an object reference, a "`_____`" is allocated to hold the value. That `_____` is an instance of a reference type, and the value is copied into that `_____`. Conversely, when an object reference is cast to a value type, a check is made that the referenced object is a `_____` of the correct value type. If the check succeeds, the value in the `_____` is copied to the value type.

%

When a value of a value type is assigned to an object reference, a "**box**" is allocated to hold the value. That **box** is an instance of a reference type, and the value is copied into that **box**. Conversely, when an object reference is cast to a value type, a check is made that the referenced object is a **box** of the correct value type. If the check succeeds, the value in the **box** is copied to the value type.

##

C#'s `_____` type system effectively means that value types are treated as object references "on demand." Because of the `_____`, general-purpose libraries that use type object can be used with all types that derive from object, including both reference types and value types.

%

C#'s **unified** type system effectively means that value types are treated as object references "on demand." Because of the **unification**, general-purpose libraries that use type object can be used with all types that derive from object, including both reference types and value types.

##

There are several kinds of `_____` in C#, including fields, array elements, local `_____`, and parameters. `_____` represent storage locations.

%

There are several kinds of **variables** in C#, including fields, array elements, local **variables**, and parameters. **Variables** represent storage locations.

##

Every variable has a type that determines what values can be stored in

%

the variable

##

A variable of "Non-nullable value type" can store

%

A value of that exact type

##

A variable of "Nullable value type" can store

%

A `null` value or a value of that exact type

##

A variable of "`object`" can store

%

A `null` reference, a reference to an object of any reference type, or a reference to a boxed value of any value type

##

A variable of "Class type" can store

%

A `null` reference, a reference to an instance of that class type, or a reference to an instance of a class derived from that class type

##

A variable of "Interface type" can store

%

A `null` reference, a reference to an instance of a class type that implements that interface type, or a reference to a boxed value of a value type that implements that interface type

##

A variable of "Array type" can store

%

A `null` reference, a reference to an instance of that array type, or a reference to an instance of a compatible array type

##

A variable of "Delegate type" can store

%

A `null` reference or a reference to an instance of a compatible delegate type
