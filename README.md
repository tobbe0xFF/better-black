![Black Logo](https://raw.githubusercontent.com/tobbe0xFF/pitch-black/master/docs/_static/logo2-readme.png)

<h2 align="center">An Uncompromising Upgrade to A Compromised Code Formatter</h2>

> “Tradition becomes our security, and when the mind is secure it is in decay."  - Jiddu Krishnamurti

_Black_ is a great code formatter... except when it is not. That is where _Pitch-Black_ comes to the rescue! By using it 
you recognise that a true craftsman cannot afford to be a slave to an arbitrary interpretation of PEP-8.

_Pitch-Black_ is based on the idea that PEP-8 is sub-optimal, and that code is more easily understood when...
 - Functions/methods are limited to as few lines as possible - as opposed to stretched out vertically
 - Function/method calls and instantiations appear clearly as discrete operations - as opposed to looking like code 
   blocks
 - Class/function/method definitions stand out as such - as opposed to looking like code blocks
 - Data structure literals (tuple, list, set, dict) are allowed to be structured to the needs - as opposed to looking 
   like code blocks
 - Trailing commas should be discouraged - as opposed to encouraged

Main features (planned):
1. By default, continuation lines should be aligned to the opening delimiter, instead of a hanging indent. This should
   go for parameter/argument lists as well as data structure literals.
   It must be possible to prevent line wrap formatting when necessary, using a manual override. That override is a 
   trailing comma in the expression. This is in contrast to the original Black where trailing commas is a manual trigger
   to _allow_ one-line formatting. The reason for this inverse behaviour is trailing commas are esthetically displeasing 
   and optimisation of formatting should be the default, not the exception. The override will respect the structure of
   the list containing the trailing comma, but will not block formatting of nested structures. This way it is possible
   to control the formatting of each nested level, when desired.
2. Default line character limit should be 120 (because most of us are not coding on CRT monitors from the 1980's)
3. Allow choice of format of indents (e.g. as number of spaces or tabs instead of the default 4 spaces)

The first two features would serve to achieve the over all goals of the fork. The third feature would serve to make the
fork more accessible to more users, since the characters used for indentation seems to be one of the main reason for
publicly available forks of Black.

The original Black repository can be found [here](https://github.com/psf/black).