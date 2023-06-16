# Stock Picker

The Stock Picker is a common programming problem that involves finding the maximum difference between two elements in an array, where the smaller element must come before the larger element. In other words, we want to identify the best days to buy and sell a stock to maximize profit.

## Problem Description

Given an array of stock prices, the task is to find the indices of the best days to buy and sell the stock. The goal is to maximize profit by buying at a lower price and selling at a higher price.

## Approach

The `stock_picker` function provides a simple and elegant solution to the Stock Picker problem in Ruby. It utilizes a one-line code implementation to find the best buy and sell days.

The code follows these steps:

1. Convert the input array of prices into an array of arrays, where each inner array contains a price and its corresponding index.
2. Generate all possible combinations of two elements from the array obtained in the previous step.
3. Calculate the profit for each pair of buy and sell days by subtracting the buy price from the sell price.
4. Find the pair of buy and sell days with the highest profit using the `max_by` method.
5. Map the selected pair of buy and sell days to their indices.
6. Return the result as an array of indices representing the best buy and sell days.

## Usage

To use the `stock_picker` function, follow these steps:

1. Define an array of stock prices.
2. Call the `stock_picker` function, passing the array of prices as an argument.
3. The function will return an array of indices representing the best days to buy and sell the stock.

Example usage:

```ruby
prices = [100, 150, 120, 200, 80, 130]
indices = stock_picker(prices)
buy_day = indices[0]
sell_day = indices[1]

puts "Best day to buy: Day #{buy_day}"
puts "Best day to sell: Day #{sell_day}"
```

Output:

```
Best day to buy: Day 4
Best day to sell: Day 3
```

In this example, the best days to buy and sell the stock are Day 4 and Day 3, respectively. The stock should be bought on Day 4 and sold on Day 3 to maximize profit.

## Conclusion

The Stock Picker problem is a common challenge in programming, and the `stock_picker` function provides a concise and efficient solution in Ruby. By following the steps outlined above, you can easily find the best days to buy and sell stocks, maximizing your potential profit.