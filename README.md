# TASK3-JPMORGAN
    my_car = Car()
print("I'm a car!")
while True:
    action = input("What should I do? [A]ccelerate, [B]rake, "
                    "show [O]dometer, or show average [S]peed?").upper()
    if action not in "ABOS" or len(action) != 1:
        print("I don't know how to do that")
        continue
    if action == 'A':
        my_car.accelerate()
        print("Accelerating...")
    elif action == 'B':
        my_car.brake()
        print("Braking...")
    elif action == 'O':
        print("The car has driven {} kilometers".format(my_car.odometer))
    elif action == 'S':
        print("The car's average speed was {} kph".format(my_car.average_speed()))
