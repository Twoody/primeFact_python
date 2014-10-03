`prime_factorization.py` includes the following:

    `is_prime`
    `pool_of_primes`
    'combinations'
    
  `is_prime`        is a normal function that tells the user if a number is prime or not.
                    It uses the concept that we only have to have a for-loop that goes
                    up to the square root of the number being entered.
  
  `pool_of_primes`  tells the user what the prime factorization of a number is
                    This is done by seeing if the number is prime by using `is_prime`.
                    If the number is not prime, we divide our number by the first
                    occurrence of a divisor. We then add this divisor to a list
                    and use recurrsion to call `pool_of_primes` again.
  
  `combinations`    combinations is the interesting feature of this program.
                    combinations returns from `pool_of_primes` a list of all divisors
                    of a number. From there, we use bitwise logic to conjure up all the
                    positive integers that divide our number (including 1 and the number
                    itself). We add these numbers to a list as we go through the bitwise 
                    logic, finally returning the list.
                    
  There are some test cses given. in `main()`
                
