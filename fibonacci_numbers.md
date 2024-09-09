import numpy as np
import pandas as pd

def Fibonacci_numbers(num):
    if num > 1:
        return Fibonacci_numbers(num-1) + Fibonacci_numbers(num-2)
    return num

def main():
    number = int(input("請輸入數列的長度:"))
    for i in range(number):
        print(Fibonacci_numbers(i), end = ", ")

if __name__ == "__main__":
    main()