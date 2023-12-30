# speedFine

def main():
    limit,clocked = eval(input("Please enter first speed limit and then clocked speed:"))
    if limit > clocked:
        if clocked < 90:
            print("The speed is legal")
        else:
            fine = 50 + 200
            print('The fine is:', fine)
    else:
        if clocked > 90:
            fine = ((clocked-limit)//5)*5 + 50 + 200
            print('The fine is:', fine)
        else:
            fine = ((clocked - limit) // 5) * 5 + 50
            print('The fine is:', fine)
main()



