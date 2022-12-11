##

C# programs run on `_____`, a virtual execution system called the `_____` and a set of `_____`.

%

C# programs run on **.NET**, a virtual execution system called the **common language runtime (CLR)** and a set of **class libraries**.

##

The CLR is the implementation by Microsoft of the common language infrastructure (CLI), an international

%

standard

##

The Common Language Infrastructure (CLI) is the basis for creating execution and development environments in which languages and libraries

%

work together seamlessly

##

Source code written in C# is compiled into an intermediate language (IL) that conforms to the Common Language Infrastructure (CLI) specification. The IL code and resources, such as bitmaps and strings, are stored in an assembly, typically with an extension of

%

.dll

##

An assembly contains a manifest that provides information about the assembly's types, version, and

%

culture

##

When the C# program is executed, the assembly is loaded into the

%

Common Language Runtime (CLR)

##

The Common Language Runtime (CLR) performs Just-In-Time (JIT) compilation to convert the Intermediate Language (IL) code to native

%

machine instructions

##

The Common Language Runtime (CLR) provides other services related to automatic garbage collection, exception handling, and resource management. Code that's executed by the CLR is sometimes referred to as

%

"managed code."

##

"Unmanaged code," is compiled into native machine language that targets a specific

%

platform

##

Language interoperability is a key feature of

%

.NET

##

Intermediate Language (IL) code produced by the C# compiler conforms to the Common Type Specification (CTS). IL code generated from C# can interact with code that was generated from the .NET versions of F#, Visual Basic, C++. There are more than 20 other

%

CTS-compliant languages

##

A single assembly may contain multiple modules written in different .NET languages. The types can reference each other as if they were written in

%

the same language

##

In addition to the run time services, .NET also includes extensive `_____`. These `_____` support many different workloads. They're organized into namespaces that provide a wide variety of useful functionality. The `_____` include everything from file input and output to string manipulation to XML parsing, to web application frameworks to Windows Forms controls.

%

In addition to the run time services, .NET also includes extensive **libraries**. These **libraries** support many different workloads. They're organized into namespaces that provide a wide variety of useful functionality. The **libraries** include everything from file input and output to string manipulation to XML parsing, to web application frameworks to Windows Forms controls.

##

The typical C# application uses the .NET class library extensively to handle common

%

"plumbing" chores
