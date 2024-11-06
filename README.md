# PY-Practical-6
str1 = input("Enter the first string: ")
str2 = input("Enter the second string: ")
n1 = int(input("Enter the number of characters to swap: "))

# Check if `n1` is valid for both strings
if n1 <= min(len(str1), len(str2)):
    # Swap the first `n1` characters
    new_str1 = str2[:n1] + str1[n1:]
    new_str2 = str1[:n1] + str2[n1:]
    print("Modified first string:", new_str1)
    print("Modified second string:", new_str2)
else:
    print("The number of characters to swap is greater than the length of one or both strings.")



'''output 
Enter the first string: hello python
Enter the second string: welcome to new world
Enter the number of characters to swap: 10
Modified first string: welcome tothon
Modified second string: hello py new world
'''
