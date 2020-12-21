# *Cryptography*

> *The Caesar Cipher technique is one of the earliest and simplest method of encryption technique. It’s simply a type of substitution cipher, i.e., each letter of a given text is replaced by a letter some fixed number of positions down the alphabet. For example with a shift of 1, A would be replaced by B, B would become C, and so on. The method is apparently named after Julius Caesar, who apparently used it to communicate with his officials.*
> *Thus to cipher a given text we need an integer value, known as shift which indicates the number of position each letter of the text has been moved down.*

``` ruby
> Text : ABCDEFGHIJKLMNOPQRSTUVWXYZ
> Shift: 23
> Cipher: XYZABCDEFGHIJKLMNOPQRSTUVW

> Text : ATTACKATONCE
> Shift: 4
> Cipher: EXXEGOEXSRGI
```
***Algorithm for Caesar Cipher:***
*Input:*

1) A String of lower case letters, called Text.
2) An Integer between 0-25 denoting the required shift.

*Procedure:*

- *Traverse the given text one character at a time.*

- *For each character, transform the given character as per the rule, depending on whether we’re encrypting or decrypting the text.*

- *Return the new string generated.*

# *Breaking the cipher*

*The Caesar cipher can be easily broken even in a ciphertext-only scenario. Two situations can be considered:*

* *an attacker knows (or guesses) that some sort of simple substitution cipher has been used, but not specifically that it is a Caesar scheme;*

* *an attacker knows that a Caesar cipher is in use, but does not know the shift value.*

> *In the first case, the cipher can be broken using the same techniques as for a general simple substitution cipher, such as frequency analysis or pattern words.[16] While solving, it is likely that an attacker will quickly notice the regularity in the solution and deduce that a Caesar cipher is the specific algorithm employed.*


# *Crash Course Computer Science*

> *Crash Course Computer Science is a series produced for the Public Broadcast System (PBS) that conveys to a broad audience of individuals Computer Science’s base knowledge. Each video is a fast paced presentation that very intentionally places basic Computer Science concepts into small, understandable segments.*

* *The running time for each video is between ten and fourteen minutes with the forty segments broken down into the following seven sections:*

*1.) The Mechanics of How Computers Work.* <br>
*2.) The Basics of Programming and Software.* <br>
*3.) Computer Hardware.* <br>
*4.) The Rise of Personal Computers and
Graphics.* <br>
*5.) The Internet* <br>
*6.) Artificial Intelligence.* <br>
*7.) Humans and the Future of Computing.*
