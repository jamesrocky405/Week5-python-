# Week5-python-

Assignment 1: Design Your Own Class – Superhero 

# Base class
class Superhero:
    def __init__(self, name, power, origin):
        self.name = name
        self.power = power
        self.origin = origin

    def introduce(self):
        print(f"I am {self.name} from {self.origin}, and I have the power of {self.power}!")

# Subclass with inheritance and polymorphism
class FlyingHero(Superhero):
    def __init__(self, name, power, origin, flight_speed):
        super().__init__(name, power, origin)
        self.flight_speed = flight_speed

    def introduce(self):  # Polymorphism: method override
        print(f"I am {self.name}, I can fly at {self.flight_speed} km/h with the power of {self.power}!")

# Creating instances
hero1 = Superhero("Shadow Knight", "invisibility", "Dark City")
hero2 = FlyingHero("Sky Falcon", "wind manipulation", "Cloud Peak", 800)

hero1.introduce()
hero2.introduce()


Activity 2: Polymorphism Challenge – Vehicles

class Vehicle:
    def move(self):
        print("Vehicle is moving...")

class Car(Vehicle):
    def move(self):
        print("Driving... ")

class Plane(Vehicle):
    def move(self):
        print("Flying... ")

class Boat(Vehicle):
    def move(self):
        print("Sailing... ")

# Polymorphic behavior
vehicles = [Car(), Plane(), Boat()]

for v in vehicles:
    v.move()


---

Would you like to add user input or create a menu for these programs?

