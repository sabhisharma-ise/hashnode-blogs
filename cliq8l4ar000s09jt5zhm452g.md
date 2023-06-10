---
title: "The all-new Enhanced Switch in Java"
datePublished: Sat Jun 10 2023 16:54:30 GMT+0000 (Coordinated Universal Time)
cuid: cliq8l4ar000s09jt5zhm452g
slug: the-all-new-enhanced-switch-in-java
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1686415860874/e870eabd-0122-4fe9-b227-3bf218946fbb.png
tags: java, switch-case, enhanced-switch

---

### **🌐 In this article, we will understand the enhanced switch, introduced in Java 13.**

## **📌 What's new**

Besides the usual way to create a switch in Java. Now you can use an arrow and yield for your switch cases. But you can also the return value from a switch case to a variable.

## **📌 Switch case with arrows**

> ### Traditional Switch

```java
public class Main {
    public static void main(String[] args) {
        String fruit = "Mango";
        switch (fruit) {
            case "Mango":
                System.out.println("Sweet and refreshing");
                break;
            case "Banana":
                System.out.println("High-fiber");
                break;
            case "Apple":
                System.out.println("Antioxidant effects");
                break;
            case "Papaya":
                System.out.println("Digestive enzymes");
                break;
            default:
                System.out.println("Eat fruits, Be Healthy!");
        }
    }
}
```

> ### Enhanced Switch

```java
public class Main {
    public static void main(String[] args) {
        String fruit = "Mango";
        switch (fruit) {
            case "Mango" -> System.out.println("Sweet and refreshing");
            case "Banana" -> System.out.println("High-fiber");
            case "Apple" -> System.out.println("Antioxidant effects");
            case "Papaya" -> System.out.println("Digestive enzymes");
            default -> System.out.println("Eat fruits, Be Healthy!");
        }
    }
}
```

> Output:-
> 
> Sweet and refreshing

### Pretty Cool isn't it?

If you use an arrow instead of a double point “:”, then you do not have to add a “break;” in every Switch case to avoid fall-through through your Switch cases. If the variable “fruit” has the value “Mango”, then case 1 with the output “Sweet and refreshing” is displayed only. You do not need a “break” in this case.

## **📌 Switch can be used as an expression**

Let’s have a look at a code snippet to understand these changes better. The yield keyword is used to return a value in a case arm that is a block of code.

```java
public class Main {
    public static void main(String[] args) {
        String fruit = "Mango";
        String selectedFruit = switch (fruit) {
            case "Mango" -> {
                yield "Mango";
            }
            case "Banana" -> {
                yield "Banana";
            }
            case "Apple" -> {
                yield "Apple";
            }
            case "Papaya" -> {
                yield "Papaya";
            }
            default -> {
                yield "";   // Empty
            }
        };
        System.out.println("Selected Fruit is " + selectedFruit);
    }
}
```

> Output:-
> 
> Selected Fruit is Mango

The switch can now be used as an expression. This means the **switch can now return values** based on our input. There is a slight change in switch syntax to accommodate this change. A switch block needs to be delimited by a semicolon. The yield keyword is used to return values. No break is required with the yield statement.

## **📌 Yield**

> ### Use of yield

```java
public class Main {
    public static void main(String[] args) {
        String fruit = "Mango";
        String selectedFruit = switch (fruit) {
            case "Mango" -> {
                System.out.println("Sweet and refreshing");
                yield "Mango";
            }
            case "Banana" -> {
                System.out.println("High-fiber");
                yield "Banana";
            }
            case "Apple" -> {
                System.out.println("Antioxidant effects");
                yield "Apple";
            }
            case "Papaya" -> {
                System.out.println("Digestive enzymes");
                yield "Papaya";
            }
            default -> {
                System.out.println("Eat fruits, Be Healthy!");
                yield "";   // Empty
            }
        };
        System.out.println("Selected Fruit is " + selectedFruit);
    }
}
```

> Output:-
> 
> Sweet and refreshing
> 
> Selected Fruit is Mango

The function “yield” can be used in a Switch statement to return a value in a switch case to a variable. We don’t need a break after yield as it automatically terminates the switch expression.

## **📌 Preview feature** 

You have to enable or add the command “ — enable-preview” in the project properties of your IDE. It does not work in some online compilers, as it is still in the experiment phase.

The enhanced switch in Java 13 provides several impressive features to the traditional switch.

Source: **Enhancements for Switch Statement in Java 13**

[https://www.geeksforgeeks.org/enhancements-for-switch-statement-in-java-13/](https://www.geeksforgeeks.org/enhancements-for-switch-statement-in-java-13/)