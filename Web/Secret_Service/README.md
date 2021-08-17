> Secret Service


## Problem

We have deciphered the Secret Service's daily color code! Every day, the Secret Service wears a special identifying pin that is the "color of the day." They use a specific algorithm to determine what the color for that day is. Can you guess what the color will be 323 days after today? Here are the clues:

The colors are: Plum, Crimson, Amethyst, Amber, White, Beige, Magenta, and Onyx in that order.
The in the list above, "Plum" is 0, "Crimson" is 1, and so on. Starting with the highest number, they add up the date (for example, 2018-10-26 would be added to 2054) and divide it by that number. If the modulus is 0, that is the color of the day. If not, they decrement by one until they reach a modulus of 0.


# Steps

1. Find the date `2022-06-30`
2. Add them `2022 + 30 + 06 = 2058`.
3. Modulo of greatest number `2058 % 6 == 0`
4. So solution is 6. And here number 6 is `Magenta`

GPSCTF{952a1af38062c22b7187c97a52ac9bec}