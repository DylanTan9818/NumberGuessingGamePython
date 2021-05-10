import random

def Guess(num):
    guess = random.randint(1,num)
     
    score = 10
    
    print('Hint:')
    
    if(guess%2 == 0):
        print("The number is even ")
    else:
        print("The number is odd")
    
    
    while(score > 0): 
        guess_num = int(input("Guess the number: "))
        if(guess_num == guess):
            print('Your guess is correct')
            break;
        elif(guess_num > guess and abs(guess - guess_num) <= 10):
            print('Your guessed number is really close. Keep going! ')
        elif(guess_num < guess and abs(guess - guess_num) <= 10):
            print('Your guessed number is really close. Keep going!')
        elif(guess_num > guess and abs(guess - guess_num) > 10 and abs(guess - guess_num) <= 50):
            print('Your guessed number is too far from the guess. Please try again')
            if(guess_num < guess and guess > 50 ):
                print('The number that you are guessing is more than 50')
            elif(guess_num > guess and guess < 50 ):
                print('The number that you are guessing is less than 50')  
        elif(guess_num < guess and abs(guess - guess_num) > 10 and abs(guess - guess_num) <= 50):
            print('Your guessed number is too far from the guess. Please try again')
            if(guess_num < guess and guess > 50 ):
                print('The number that you are guessing is more than 50')
            elif(guess_num > guess and guess < 50 ):
                print('The number that you are guessing is less than 50')
                
        score-=1
        print(f"Your total score left is {score}")
    
    if(score == 0):    
        print("Game over")
    else:
        print(f"Hooray! Your final score is {score}")

num = int(input("Enter range of number from 1 to 100: "))
Guess(num)
