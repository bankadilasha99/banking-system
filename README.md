# banking-system
#a small responsive banking system project.. 
  #function
  
def bank():                

    while True:          #to run infinite times
    
        print('1.new customer')
        print('2.existing customer')
        print('3.exit')
        "-----------------------------------"
        
        option=int(input('Enter choice:'))
       
       if option==1:                            
            account=int(input('Enter your account number:'))
            name=input('Enter your name:')
            address=input('Enter your address:')
            phone=int(input('Enter your phone number:'))
            govt_id=input('Enter Govt ID:')
            acctype=input('Enter Account type:')
            amount=int(input('Enter Amount:'))
            print('Account Successfully Created')
        elif option==2:
                accountno=int(input('Enter your account number:'))
                if accountno!=account:
                    print('record not found')
                else:
                    print('Record  found')
                    print('1.Check Balance')
                    print('2.Withdraw')
                    print('3.Deposit')
                    "-------------------------------------------"
                    option1=int(input('Enter choice:'))
                    "--------------------------------------------"
                    if option1==1:
                        balance=int(input('balance to be depasited:'))
                        print('your balance is:',amount+balance)
                    if option1==2:
                        withdraw=int(input('Enter your balance to withdraw:'))
                        "----------------------------------------------------"
                        print('Withdraw Sucessful')
                        print('Available Balance:',amount-withdraw)
                    if option1==3:
                        deposit=int(input('Enter amount to deposit:'))
                        "---------------------------------------------------"
                        print('Deposit Sucessful')
                        print('Available Balance:',amount+deposit)
        elif(option==1 or option==2):
            continue
        else:
            break

bank()
