# Simple Python Script for the Password Validation.



````
min_digits = 3
min_alphas = 3
min_length = 8

password = input('Enter Your Password : ')

digit_counter =0
alpha_counter = 0

if len(password) >= min_length:
    
    for char in password:
        
        if char.isdigit():
            digit_counter = digit_counter + 1
        
        elif char.isalpha():
            alpha_counter = alpha_counter + 1
    
    if alpha_counter >= min_alphas and digit_counter >= min_digits:
        print('Validation ok')
    
    else:
        print('validation failed')
else:
    print('Password length does not match')
    
````
    
    
    

# Result

````
Enter Your Password : test123456
Validation ok

````
