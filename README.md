# guessing_game
Guess the correct number between 0-10!

from random import randint

def gg():
    answer=randint(0,10)
    name=input('Please enter your name: ')

    #If the user leaves their name blank, have a message here
    while len(name)==0:
        print ('I am sure you have a name!')
        name=input('Please enter your name: ')
        
    guess=int (input('please enter an integer from %d to %d:'%(0,10)))

    

    
    while (guess!= answer):
        if (guess > answer):
            print('the correct answer is lower')
            guess=int (input('please enter an integer from %d to %d:'%(0,10)))

        else:
            print ('the correct answer is higher')
            guess= int(input('please enter an integer from %d to %d:'%(0,10)))
    else:
        print ('Congratulations you are a winner!')








    
