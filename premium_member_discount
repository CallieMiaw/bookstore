# Program Description: A bookstore asked me to help with programming their cashiering machine after
# They  developed a program to encourage their customers to purchase many books at a time to increase sales.
# They have also created a membership program to provide even better deals for their premium customers.


def main():
    #collecting user input
    name = input("What is your name? ")
    num_books = int(input("How many books would you like to buy? "))
    member_type = input("What kind of member are you? (Press R for Regular or P for Premium): ")
    membership_fee = 0
    if member_type in "Rr":
        upgrade = input("Would you like to upgrade to a premium membership for a fee of $4.95? (Y for Yes or N for No): ")
        if upgrade in "Yy":
            member_type = "P"
            membership_fee = 4.95



    #calculating free books so that I can find the number of books the buyer has to pay for
    if member_type in "Pp":
        membership = "Premium"
        cost_per_book = 8.49
        if num_books < 6:
            free_books = 0
        if (num_books >= 6) and (num_books <= 9):
            free_books = 1
        else:
            free_books = 2

    if member_type in "Rr":
        membership = "Regular"
        cost_per_book = 9.95
        if num_books < 8:
            free_books = 0
        if (num_books >= 8) and (num_books <= 12):
            free_books = 1
        else:
            free_books = 2



    #calculations to determine the cost
    #using format function to accurately round the decimal place for change
    total_books = num_books + free_books
    sub_total = format(num_books * cost_per_book, '.2f')
    tax = format((float(sub_total) * .0825), '.2f')
    total = format(float(sub_total) + float(tax) + float(membership_fee), '.2f')




    #printing the outputs to the buyer
    print("\n-------Product Summary-------")
    print("Customer Name:", name)
    print("Customer Type:", membership)
    print("Total Books:", str(total_books))
    print("Subtotal: $" + str(sub_total))
    if upgrade in "Yy":
        print("Thank you for upgrading to premium membership")
        print("Membership fee: $" + str(membership_fee))
    print("Tax: $" + str(tax))
    print("Total: $" + str(total))

main()



