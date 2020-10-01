# SNAKKE WATER GUN GAME
print(" WELCOME TO THE SNAKE WATER GUN GAME \n"
      "press S for snake\n"
      "      w for water\n"
      "      g for gun ")
import random
list = ["snake", "gun", "water"]
n = 10
m=0
user=0
comp=0
while m<n:
    a = str(input("type here:"))
    b = random.choice(list)
    if a == b:
        print("the game is tied\n")
    elif a == "s" and b=="water":
        user = user+1

        print(f"you won this turn")
        print(f"your score is {user} and opponent score is {comp}")
        print(f"your input is {a} and opponent says {b}")
    elif a == "s" and b=="gun":
        comp = comp +1
        print(f"you lost this time")
        print(f"your score is {user} and opponent score is {comp}")
        print(f"your input is {a} and opponent says {b}")
    elif a == "w" and b == "gun":
        user = user + 1
        print(f"you won this turn")
        print(f"your score is {user} and opponent score is {comp}")
        print(f"your input is {a} and opponent says {b}")
    elif a == "w" and b== "snake":
        comp = comp +1
        print(f"you lost this time")
        print(f"your score is {user} and opponent score is {comp}")
        print(f"your input is {a} and opponent says {b}")
    elif a == "g" and b=="snake":
        user = user + 1
        print(f"you won this turn")
        print(f"your score is {user} and opponent score is {comp}")
        print(f"your input is {a} and opponent says {b}")
    elif a == "g" and b== "water":
        comp = comp + 1
        print(f"you lost this time")
        print(f"your score is {user} and opponent score is {comp}")
        print(f"your input is {a} and opponent says {b}")
    else:
        print("you have given wrong input")
    m=m+1
    print(f"{n-m} chances are left out of 10")
if user>comp:
    print("you won this game\n"
          "VICTORY")
else:
    print("you lost this game\n"
          "better luck next time\n"
          "GAME OVER")




