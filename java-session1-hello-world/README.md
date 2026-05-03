# Java Session 1 – Hello World

## What is Java?

Java is a high-level, object-oriented programming language developed by Sun Microsystems (now owned by Oracle) in 1995. It follows the principle of **"Write Once, Run Anywhere"** — code you write on one machine can run on any device that has a Java runtime installed, without modification.

Java is widely used for building desktop applications, web backends, Android apps, enterprise systems, and more.

---

## JDK, JRE, and JVM — What's the Difference?

### JVM — Java Virtual Machine
The **JVM** is the engine that actually runs your compiled Java code. It reads Java bytecode (`.class` files) and executes it on the underlying operating system. The JVM is what makes Java platform-independent — the same bytecode runs on Windows, macOS, or Linux as long as a JVM is installed.

### JRE — Java Runtime Environment
The **JRE** is a package that includes the JVM plus the standard Java class libraries needed to *run* Java programs. If you only need to run Java applications (not develop them), the JRE is all you need.

### JDK — Java Development Kit
The **JDK** is the full toolkit for *developing* Java programs. It includes:
- The JRE (and therefore the JVM)
- A compiler (`javac`) to turn `.java` source files into `.class` bytecode
- Debugging and development tools

**Summary:**

| Component | Contains | Used For |
|-----------|----------|----------|
| JVM | Bytecode executor | Running bytecode |
| JRE | JVM + standard libraries | Running Java programs |
| JDK | JRE + compiler + dev tools | Writing & running Java programs |

> If you are writing Java code, you need the **JDK**.

---

## How to Compile and Run a Java Program

### Step 1 – Write your source file
Create a file named `HelloWorld.java` (the filename must match the class name exactly).

### Step 2 – Compile with `javac`
Open a terminal in the same directory as your file and run:

```bash
javac HelloWorld.java
```

This produces a `HelloWorld.class` file containing bytecode.

### Step 3 – Run with `java`

```bash
java HelloWorld
```

Do **not** include the `.class` extension when running. You should see:

```
Hello, World!
```

---

## HelloWorld.java

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

- `public class HelloWorld` — defines a class named `HelloWorld`
- `public static void main(String[] args)` — the entry point every Java program starts from
- `System.out.println(...)` — prints a line of text to the console
