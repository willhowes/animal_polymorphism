### Animal Polymorphism

This is an example of polymorphism and duck-typing.

It shows that you can have many classes which have similar but not exactly the same attributes (in this example, animals). The attributes which are common can be held in a separate class (in this case the ```Animal``` class)

Here the ```Animal``` class has a method ```make_noise```. All animals, as far as I am aware, makes noises but these are different depending on the animal. So in this example we use polymorphism since an animal has "many forms" (or "poly morph"). This ``make_noise`` method in the ```Animal``` class works because of duck-typing, since ```make_noise``` on an instance of the ```Animal``` class will accept any object given to it which has a make_noise method.  

When we call the make_noise method on a new instance of ```Animal``` with an instance of a ```Dog``` or ```Cat``` class the method works since the ```Dog``` and ```Cat``` classes have a make_noise method.

However, if we try to call the make_noise method passing an instance of the ```SilentAnimal``` class then we get the following error: ```(undefined method 'make_noise' for #<SilentAnimal:0x00007fd2ea097558>)```

Since the ```SilentAnimal``` class does not have a make_noise method.

This example was given to me by my excellent peer at [Makers Academy](https://makers.tech/) https://github.com/zi-codes .
