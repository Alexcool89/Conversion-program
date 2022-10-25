# Conversion-program
This is a conversion program Euro->lei or Lei->Euro

print("Hello! \nThis is a conversion program Euro->lei or Lei->Euro")
currencyChoice = input(

    "\nWrite L for conversion Euro->Lei and E for conversion  Lei->Euro:\n")
    
currencyChoice = currencyChoice.upper()

if (currencyChoice.isalpha()):
    if (currencyChoice == 'L'):
        euro = input("\nWrite the number of euros you want to convert:\n")
        if (euro.isdigit()):
            euro = int(euro)
            print("The converted value is :", f'{euro*4.92:.2f}', " RON")
        else:
            print("The entered value is not a number!")

    elif (currencyChoice == "E"):
        lei = input("\nWrite the number of Lei you want to convert:\n")
        if (lei.isdigit()):
            lei = int(lei)
            print("The converted value is :", f'{lei/4.92:.2f}', " EURO")
        else:
            print("The entered value is not a number!")

    else:
        print("The entered value is not recognized!")
else:
    print("The entered value is not an alpha character!")

input("\nPress <enter> to exit.")
