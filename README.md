# Abstraction-Summative
Pizza Ordering System Code

def wronginput():
    print("Wrong Input!")
    exit()


def abstraction():
    pizzalist=[]
    pizzacost=[]

    number = int(input(("Would you like pizza?\n"
          "1 = yes\n"
          "2 = no")))
    if number not in [1,2]:
        wronginput()

    if number == 2:
        exit()

    if number == 1:
        dough = int(input(("What dough would you like?\n"
                       "1 = regular\n"
                       "2 = whole_wheat")))
        if dough not in [1,2]:
            wronginput()

        if dough == 1:
            pizzalist.append("Regular dough")
            pizzacost.append(5)
        if dough == 2:
            pizzalist.append("Whole wheat dough")
            pizzacost.append(7)
        if dough == 1 or 2:
            sauce = int(input(("What sauce would you like?\n"
                               "1 = tomato\n"
                               "2 = chilli")))
            if sauce not in [1, 2]:
                wronginput()
            if sauce == 1:
                pizzalist.append("Tomato sauce")
                pizzacost.append(3)
            if sauce == 2:
                pizzalist.append("Chilli sauce")
                pizzacost.append(6)
            if sauce == 1 or 2:
                cheese = int(input(("What cheese would you like?\n"
                                    "1 = parmesan\n"
                                    "2 = mozzerella")))
                if cheese not in [1, 2]:
                    wronginput()
                if cheese == 1:
                    pizzalist.append("Parmesan cheese")
                    pizzacost.append(4)
                if cheese == 2:
                    pizzalist.append("Mozzerella cheese")
                    pizzacost.append(4)
                if cheese == 1 or 2:
                    toppings = int(input(("What toppings would you like?\n"
                                          "1 = olives\n"
                                          "2 = tomatos")))
                    if toppings == 1:
                        pizzalist.append("Olive topping")
                        pizzacost.append(2)
                    if toppings == 2:
                        pizzalist.append("Tomato topping")
                        pizzacost.append(2)
                    if toppings == 1 or 2:
                        print(pizzalist)
                        print(pizzacost)

abstraction()
