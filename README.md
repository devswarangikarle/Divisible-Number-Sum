# Divisible-Number-Sum
You are given a positive integer n. Your task is to write a function that calculates the sum of all integers in the range [1, n] inclusive, which are divisible by 2, 3, or 7. Determine the sum of all numbers in the given range satisfying the constraint.

def divisible_number_sum(n):
    sum = 0
    for i in range(1, n+1):
        if i % 2 == 0 or i % 3 == 0 or i % 7 == 0:
            sum += i
    return sum

n = int(input())

print(divisible_number_sum(n))
