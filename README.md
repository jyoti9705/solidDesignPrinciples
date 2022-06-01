# solidDesignPrinciples

1. Liskov Substitution Principle
    1. Definition
        1. let's say we have a class of type T and a subtype of T which is S , Liskov Substitution Principle states that
           if S is Subtype of T and T has some property x then S should by default have that property.
        2. It is trying to explain us when to use Inheritance and when to not
    2. Example
        1. If we have a class Animal, and it has a property eat now lets say we have a subclass Frog then Frog should
           default have the property of eating , if it is not then we are breaking the principle
2. Interface Segregation Principle
    1. Definition
        1. As per this principle it is better to have many small interfaces rather than having one large interface which
           binds every implementing class to override all the methods in it
        2. Advantages of Doing it
            1. By implementing small interfaces over large one we are favouring composition over Inheritance and
               Decoupling over coupling
            2. We can have additional interfaces added without hampering the existing ones
        3. Example
            1. We have an Animal Interface with methods eat , sleep , move as per this principle instead of eat , move
               and sleep in one interface it is better to have 3 separate interfaces like IEat , IMove, ISleep and then
               implement those methods
3. Dependency Inversion Principle
    1. Definition
        1. High level modules should not depend on low level modules, both should depend on abstraction , Abstraction
           should not depend upon details , Details should be dependent on abstraction
        2. So th point of having Dependency Inversion is that you can change behaviour of your program at Runtime
           instead of compile time
    2. Advantages
        1. Easy to use
        2. Increase flexibility and reuse of the code
        3. Small classes with limited responsibility which can change with other classes
        4. Without Dependency Inversion Testing will be difficult
            1. This helps in complete isolation
4. Open Closed Principle
    1. We should avoid rewriting code anyhow
    2. We can add delete independently
    3. We should try to reuse the code as much as possible
    4. Wrote new code instead of changing the old one
5. Single Responsibility Principle
    1. Definition
        1. A single module of class or the code should be responsible for single responsibility
            1. What is a Single thing?
                1. A class or module should have a single reason to change
                2. Assume you have a system and people come to you desk and ask to change a different people will have
                   different requirements, if you're building your own products then we will have to vision these
                   requests before, so it is better to develop the code in a way that we have only single reason to
                   change