# function to create acronym
def function(string):
    # add first letter
    output = string[0]

    # iterate over string
    for i in range(1, len(string)):
        if string[i - 1] == ' ':
            # add letter next to space
            output += string[i]

    # uppercase output
    output = output.upper()
    return output


# input string
input1 = input("Enter a string: ")
# output acronym
print(function(input1))

