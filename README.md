# subtask2
def calculate_quotient_remainder(a, b):
    # Check if b is 0
    if b == 0:
        return -1, -1
    
    # Initialize variables
    q = 0
    r = a
    
    # Loop to calculate quotient and remainder
    while r >= b:
        q += 1
        r -= b
    
    return q, r

# Example usage
a = 13
b = 5

quotient, remainder = calculate_quotient_remainder(a, b)

# Output results
print(f"For a={a} and b={b}, Quotient (q): {quotient}, Remainder (r): {remainder}")
