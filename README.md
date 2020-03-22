# Trivia-Game-Calculator
Integration Project that features a 4 function calculator and a trivia game
#Christina Aragon
# Guessing Game with a Calculator

   
#16 Lines
def main():
    print("Welcome to the Guessing Game of the century! All characters are case sensitive so watch out!")
    useranswer = input("Are you ready to play? Yes, No? If a Calculator is needed type Calculator.  Type Choice Here:")

#SOME VARIABLES
#Sports

    answerSport1 = "Kansas City Chiefs"
    answerSport2 = "4"

#Tech

    answerTech2 = "2025"
    answerTech1 = "Elon Musk"


#FOR USER TO BEIGIN THE GAME
    if useranswer == "Yes":
        start = print("Lets Begin! ")
    
            input("Topic Choices: Sports Trivia or Technology Fun Facts? Press Enter to continue ")
            topic1 = "Sports Trivia"
            topic2 = "Technology Fun Facts"
            topic3 = "National Park Trivia"
            topic = ""
            topic = input("Enter Topic Choice: ")
    
#SPORTS TRIVIA
    #FIRST QUESTION
    #Ryan the TA helped guide me
        if topic == "Sports Trivia":
        # How to automatically have Enter Guess pop up

        
            sportquestion1 = input("Who won the most recent Superbowl? Press Enter to beign. ")
            answerSport1 = "Kansas City Chiefs" or "The Chiefs" or "Chiefs" #figure out how to let the user have some leeway
            guess = ""
            guess_count = 0
            guess_limit = 3
            out_of_guesses = False
        
# 10 Lines

            while guess != answerSport1 and not(out_of_guesses):
                if guess_count < guess_limit:
                    guess = input("Enter guess: ")
                    guess_count += 1
                else:
                    out_of_guesses = True
            if out_of_guesses:
                print("YOU LOSE! Come Back Next Time! ")
            else:
                print("Good Job!")
            

#17 Lines
#SPORTS
#SECOND QUESTION 
            if guess == answerSport1:
                sportquestion2 = input("The Olympics are held every how many years? Press Enter to Beign. ")
                answerSport2 = "4" or "4 years" or "4 Years"
                guess = ""
                guess_count = 0
                guess_limit = 3
                out_of_guesses = False

                while guess != answerSport2 and not(out_of_guesses):
                    if guess_count < guess_limit:
                        guess = input("Enter guess: ")
                        guess_count += 1
                    else:
                        out_of_guesses = True
    
                if out_of_guesses:
                    print("YOU LOSE! Come Back Next Time")
                else:
                    print("You Won! ")
                
# 17 Lines
#TECHNOLOGY
#FIRST QUESTON
        elif topic == "Technology Fun Facts":
        # How to automatically have Enter Guess pop up
            techQuestion1 = input("Who owns Space X and Tesla? Press Enter to continue. ")
            answerTech1 = "Elon Musk"
            guess = ""
            guess_count = 0
            guess_limit = 3
            out_of_guesses = False
#   
            while guess != answerTech1 and not(out_of_guesses):
                if guess_count < guess_limit:
                    guess = input("Enter guess: ")
                    guess_count += 1
                else:
                    out_of_guesses = True
        if out_of_guesses:
            print("YOU LOSE! Come Back Next Time! ")
        else:
            print("Good Job!" + "You are doing amazing sweetie!")

# 17 lines
#TECHNOLOGY
#SECOND QUESTION

            if guess == answerTech1:
                techquestion2 = input("When are we suppose to go to the Mars? Press Enter to Beign. ")
                answerTech2 = "2025"
                guess = ""
                guess_count = 0
                guess_limit = 3
                out_of_guesses2 = False

                while guess != answerTech2 and not(out_of_guesses):
                    if guess_count < guess_limit:
                        guess = input("Enter guess: ")
                        guess_count += 1
                    else:
                        out_of_guesses = True

                if out_of_guesses2:
                    print("YOU LOSE! Come Back Next Time")
                else:
                    print("You Won! " + "Have a great day!")

                        
#CALCULATOR
#POGIL 
                
    elif useranswer == "Calculator":
        print("Welcome to the Calculator. ")
        function = input("What Function would you like to do? Add, Subtract, Multiply, Divide.")
            
        if function == "Add":
            print("Now enter your two values.. ")
            
            num1=int(input("First Number: "))
            num2=int(input("Second number: "))
            
            sum= float(num1) + float(num2)
            print('The Total of {0} and {1} is {2}'.format(num1, num2, sum))
            
        elif function == "Subtract":
            print("Now enter your two values.. ")
            
            num1=int(input("First Number: "))
            num2=int(input("Second number: "))
            
            sum= float(num1) - float(num2)
            print('The Value of {0} and {1} is {2}'.format(num1, num2, sum))
            
        elif function == "Multiply":
            print("Now enter your two values.. ")
            
            num1=int(input("First Number: "))
            num2=int(input("Second number: "))
            
            sum= float(num1) * float(num2)
            print('The Value of {0} and {1} is {2}'.format(num1, num2, sum))
            
        elif function == "Divide":
            print("Now enter your two values.. ")
            
            num1=int(input("First Number: "))
            num2=int(input("Second number: "))
            
            sum= float(num1) / float(num2)
            print('The value of {0} and {1} is {2}'.format(num1, num2, sum))
        else:
            print("It was nice knowing you! ")
        
#END
    
    else:
        print("Come Back Soon!")

####### CALL TO MAIN ######
main()


