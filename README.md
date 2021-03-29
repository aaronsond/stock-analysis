# stock-analysis

## Overview

This analysis looks at volume and return on certain stocks over a given year with given data. This will help in making investment decisions. The project also contains modular code that should make it easy to edit, or run further analysis on similarly formatted data in the future. 

## Results

### 2017

The selected stocks performed, on average, much better in 2017 than 2018. 

(Results and runtime from 2017)[Resources/VBA_Challenge_2017.png]

All of the sampled green stocks had positive returns in 2017, aside from TERP, which had a low negative return. DQ, SEDG, ENPH and FSLR all had returns above 100%. 

### 2018

The runtime for the code in 2018 was 0.15625, less than 2/10 of a second.

(Results and runtime from 2018)[Resources/VBA_Challenge_2018.png]

By contrast, the returns in 2018 on the same stocks were on average megative. RUN and ENPH continued to turn profitable, with a much better year for RUN than 2017, but the rest of the stocks listed were in negative returns. 

The runtime for the code in 2018 was 0.1484375, slightly faster than for the data in 2017

## Summary 

### Notes on Refactoring code

Refactoring code comes with strengths; the cose will run faster, making it more time efficient, and often also makes the code clearer and easier to manage for future uses. The disadvantage is that it is time consuming. Going back through code and finding new and better ways to solve the same problem can take a lot of time, and ensuring that the new version is correct is tricky, and takes focus. If you have a deliverable that is needed in a short timeframe, refactoring your code may not be a realistic option.

### Refactoring code for stock analysis

In this context, the code used had nested `For` loops, which mean it ran through the code thousands of times more than needed. When we refactored it, we used a ticker index, which allowed it to run wihout the nested loops. It runs faster, is cleaner, and easier to understand. However, both versions of the code performed the same critical function, and in this size of a data set, the delay in processing the code is not critical. It will work better and faster when retooled to work with a different dataset.