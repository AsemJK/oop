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

Encapsulation is the ability of an object to hide parts of its state and behaviors from other objects, exposing only a limited interface to the rest of the prgram.

Example:
You have a car, To start engin you only need to turn a key or press start button right? you don't need to know about wires under the hood or crankshaft or even cylinders, so you have a simple **interface** contains a start switch, a steering wheel and some pedals.
__Interface__ is the public part of an object and open the interactions with other objects.

الخلاصة:
في هذا الجزء من نموذج البرمجة كائنية التوجه نقول أن العنصر يجب أن يكون فيه آلية لإخفاء و إظهاء الخصائص و الأفعال داخله و تكون هناك فقط واجهة له تحدد سياسة تفاعله مع العناصر الأخرى في التطبيق

### Inheritance

Inheritance is a mechanism by which one class (child / derived) acquires the properties and behaviors of another class (parent / base).  
It lets you define a new class that _reuses_, extends or modifies the behavior of the existing class without touching its code.

Example:  
We already have a base class `Vehicle` that contains general properties: `speed`, `weight`, `fuelCapacity`, and a method `move()`.  
When we need a `Plane` we do NOT copy-paste all of that code; instead we **inherit** from `Vehicle` and add only the extras that are specific to a plane: `altitude`, `pitchAngle`, `takeOff()`, `land()`.

If tomorrow we build `Car` or `Boat` we still inherit from the same `Vehicle`, guaranteeing that every vehicle in our program already “knows” how to `move()` while allowing each subclass to specialize further.

الخلاصة:  
الوراثة تسمح لك بإنشاء كلاس جديد يعيد استخدام كل الخصائص والوظائف الموجودة في كلاس آخر ويضيف إليها ما يلزم، مما يقلل التكرار ويزيد من إعادة استخدام الشيفرة.
