How to Calculate Password Entropy?
Password entropy predicts how difficult a given password would be to crack through guessing, brute force cracking, dictionary attacks or other common methods. Entropy essentially measures how many guesses an attacker will need to make to guess your password.

As computing power grows, the amount of time required to guess large amounts of passwords decreases significantly, therefore it is useful to make certain assumptions at the time of a given calculation as to number of guesses per second a computer can make (a factor which varies over time).

The number of guesses it takes to 100% definitely guess a password or passphrase (i.e. number of possible password or passphrase combinations) typically tends to be a function of the size of the “symbol pool” to the power of the number of symbols used.

Entropy Formula
L = Password Length; Number of symbols in the password

S = Size of the pool of unique possible symbols (character set).

For example:

Numbers (0-9): 10
Lower Case Latin Alphabet (a-z): 26
Lower Case & Upper Case Latin Alphabet (a-z, A-Z): 52
ASCII Printable Character Set (a-z, A-Z, symbols, space): 95
Number of Possible Combinations = SL

Entropy = log2(Number of Possible Combinations)

It is important to note that statistically, a brute force attack will not require guessing ALL of the possible combinations to eventually hit the right permutation. We therefore tend to look at the expected number of guesses required which can be rephrased as how many guesses it takes to have a 50% chance of guessing the password.

This can be expressed by extending the formula above:

Expected Number of guesses (to have a 50% chance of guessing the password) = 2Entropy-1

Examples
The following table illustrates some examples of entropy calculations of passwords of varying strength:

Complexity	Entropy Calculation
4 characters consisting of:
Letters of the same case
Length: 4
Possible Symbols: 26
Possible combinations: 264 = 456,976
Bits of Entropy: log2(264) = 18.80
Strength: Very Weak
8 characters consisting of:
Letters of the same case
Length: 8
Possible Symbols: 26
Possible combinations: 268 = 208,827,064,576
Bits of Entropy: log2(268) = 37.60
Strength: Weak
8 characters consisting of:
Letters (upper and lower case)
Length: 8
Possible Symbols: 52
Possible combinations: 528 = 9.1343852e+46
Bits of Entropy: log2(528) = 45.60
Strength: Reasonable
8 characters consisting of:
Letters (upper and lower case)
Numbers
Length: 8
Possible Symbols: 62
Possible combinations: 628 = 2.1834011e+14
Bits of Entropy: log2(628) = 47.63
Strength: Reasonable
8 characters consisting of:
Letters (upper and lower case)
Numbers
Symbols
Length: 8
Possible Symbols: 95
(assuming ASCII Printable Characters set)
Possible combinations: 958 = 6.6342043e+15
Bits of Entropy: log2(958)= 52.56
Strength: Reasonable
5 random words taken from:
the Diceware™ wordlist, or
the EFF word list
Length: 5
Possible Symbols: 7776
(assuming no capitalization variations are used)
Possible combinations: 77765 = 2.8430288e+19
Bits of Entropy: log2(77765) =64.62
Strength: Strong
However, this formula would only apply to the simplest of cases. Many online password meters and registration forms complicate matters by imposing various arbitrary (and unfortunately non-random) restrictions on allowed patterns which may exist in a password. Examples include “at least one upper-case character”, “at least one symbol” etc.

While initially designed in the efforts to reduce the risks of social engineering or dictionary attacks, it turns out that in many cases, this may cause a degradation in password strength. Click to read more on why password strength rules are not so great after all.

© Generate Passwords 2022 - All right reserved
