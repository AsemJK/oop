# oop
Here I will simplify OOP as possible as can, with real examples

## Pillars
### Abstraction

Abstraction is a model of a real-world object or phenomenon,
limited to a specific context, which represents all details relevant
to this context with high accuracy and omits all the rest.

Example:
When we create a class to represent a "Plane"
Plane has a huge number of properties: seats, speed, altitude,pitchAngle ,...

When we want to use this "interface" in booking system then no need to use property like "altitude" right? here we absolutely need "seats" property,but when we making a simulation system for flying then we need some engineering information like speed, altitude,...

This is abstraction, for object show only what you need based on context.

الخلاصة:
التجريد يساعد على وجود كلاس بخصائص مختصرة و واضحة مرئية فقط لمن يحتاجها من العناصر في التطبيق

### Encapsulation

Encapsulation is the ability of an object to hide parts of its sate and behaviors from other objects, exposing only a limited interface to the rest of the prgram.

