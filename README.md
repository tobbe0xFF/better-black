![Black Logo](https://raw.githubusercontent.com/tobbe0xFF/pitch-black/master/docs/_static/logo2-readme.png)

<h2 align="center">An Uncompromising Upgrade to A Compromised Code Formatter</h2>

> “Tradition becomes our security, and when the mind is secure it is in decay."  - Jiddu Krishnamurti

_Black_ is a great code formatter... except when is not. That is where _Pitch-Black_ comes to the rescue! By using it 
you recognise that a true craftsmans must not be a slave to an arbitary interpretation PEP-8.

_Pitch-Black_ is based on the idea that code is more understandable when...
 - Discrete operations appear clearly as discrete operations (not like code blocks)
 - Functions/methods are limited to fewer lines each (as opposed to stretched out vertically)

.

Main goals (features):
1. By default, continuation lines should be alignment to the opening delimiter, instead of a hanging indent. This should
   go for parameter lists and argument lists, as well as for elements in containers (such as lists, tuples, dictionaries
   etc). 
   It should be possible to manually override this when necessary, by using a trailing comma. Such an override would 
   leave the present line continuation untouched for that specific expression, in respect to it's elements, but would 
   not stop formatting of expressions amounting to elements, themselves.
2. Default line character limit should be 120 (because most of us are not coding on CRT monitors from the 1980's)

These two changes would serve to achieve the over all goals of the fork.

.

Stretch goals (features):
3. Allow defining indents as number of spaces or tabs instead of the default 4 spaces

This change would serve to make the fork more accessible to more users, since the characters used for indentation seems
to be one of the main reason for forking Black in general.

.

The original Black repository can be found [here](https://github.com/psf/black).