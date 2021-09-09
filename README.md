# Rock_Paper_Scissors

print("Welcome to the game of Rock, Paper and Scissors")

print("\n")

player1 = str(input("Enter your Name: "))
player2 = str(input("Enter your Name: "))

print("\n")
print("-"*60)

i = 0

play1 = 0
play2 = 0

while (i<3):
    print("Round: ", i+1)
    p1 = str(input(player1 + ", Enter your Choice (Rock/Paper/Scissors): "))
    p2 = str(input(player2 + ", Enter your Choice (Rock/Paper/Scissors): "))
    
    if p1 == p2:
        print("It's a Tie")
        play1 = play1 + 0.5
        play2 = play2 + 0.5
        print("The score of ", player1, "is ", play2,".")
        print("The score of ", player2, "is ", play2,".")
        print("\n")

    elif p1 == "Rock":
        if p2 == "Paper":
            print("Paper covers Rock. ", player2, "win the game")
            play2 = play2 + 1
            print("The score of ", player1, "is ", play1,".")
            print("The score of ", player2, "is ", play2,".")
            print("\n")
        else:
            print("Rock smashes Scissors. ", player1, "win the game")
            play1 = play1 + 1
            print("The score of ", player1, "is ", play1,".")
            print("The score of ", player2, "is ", play2,".")
            print("\n")

    elif p1 == "Paper":
        if p2 == "Rock":
            print("Paper covers Rock. ", player1, "win the game")
            play1 = play1 + 1
            print("The score of ", player1, "is ", play1,".")
            print("The score of ", player2, "is ", play2,".")
            print("\n")
        else:
            print("Scissors cut Paper. ", player2, "win the game")
            play2 = play2 + 1
            print("The score of ", player1, "is ", play1,".")
            print("The score of ", player2, "is ", play2,".")
            print("\n")

    elif p1 == "Scissors":
        if p2 == "Rock":
            print("Rock smashes Scissors. ", player2, "win the game")
            play2 = play2 + 1
            print("The score of ", player1, "is ", play1,".")
            print("The score of ", player2, "is ", play2,".")
            print("\n")
        else:
            print("Scissors cut Paper. ", player1, "win the game")
            play1 = play1 + 1
            print("The score of ", player1, "is ", play1,".")
            print("The score of ", player2, "is ", play2,".")
            print("\n")
   
    else:
        print("Please enter valid Choice. ")
        
    i = i + 1
    
print("-"*60)
print("Thanks for playing")
