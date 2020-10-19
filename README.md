# Object-Oriented-Programming



Dr. Alan Kay on the Meaning of “Object-Oriented Programming”

E-Mail of 2003-07-23
Dr. Alan Kay was so kind as to answer my questions about the term “object-oriented programming”.  
Date: Wed, 23 Jul 2003 09:33:31 -0800

******************************
To: Stefan Ram [removed for privacy]

From: Alan Kay [removed for privacy]

Subject: Re: Clarification of "object-oriented"

[some header lines removed for privacy]

Content-Type: text/plain; charset="us-ascii" ; format="flowed"

Content-Length: 4965

Lines: 117



Hi Stefan --



Sorry for the delay but I was on vacation.



At 6:27 PM +0200 7/17/03, Stefan Ram wrote:

>   Dear Dr. Kay,

>

>   I would like to have some authoritative word on the term

>   "object-oriented programming" for my tutorial page on the

>   subject. The only two sources I consider to be "authoritative"

>   are the International Standards Organization, which defines

>   "object-oriented" in "ISO/IEC 2382-15", and you, because,

>   as they say, you have coined that term.



I'm pretty sure I did.



>

>   Unfortunately, it is difficult to find a web page or source

>   with your definition or description of that term. There are

>   several reports about what you might have said in this regard

>   (like "inheritance, polymorphism and encapsulation"), but

>   these are not first-hand sources. I am also aware that later

>   you put more emphasis on "messaging" - but I still would like

>   to know about "object oriented".

>

>   For the records, my tutorial page, and further distribution

>   and publication could you please explain:

>

>     When and where was the term "object-oriented" used first?



At Utah sometime after Nov 66 when, influenced by Sketchpad, Simula, 

the design for the ARPAnet, the Burroughs B5000, and my background in 

Biology and Mathematics, I thought of an architecture for 

programming. It was probably in 1967 when someone asked me what I was 

doing, and I said: "It's object-oriented programming".



The original conception of it had the following parts.



  - I thought of objects being like biological cells and/or individual 

computers on a network, only able to communicate with messages (so 

messaging came at the very beginning -- it took a while to see how to 

do messaging in a programming language efficiently enough to be 

useful).



  - I wanted to get rid of data. The B5000 almost did this via its 

almost unbelievable HW architecture. I realized that the 

cell/whole-computer metaphor would get rid of data, and that "<-" 

would be just another message token (it took me quite a while to 

think this out because I really thought of all these symbols as names 

for functions and procedures.



  - My math background made me realize that each object could have 

several algebras associated with it, and there could be families of 

these, and that these would be very very useful. The term 

"polymorphism" was imposed much later (I think by Peter Wegner) and 

it isn't quite valid, since it really comes from the nomenclature of 

functions, and I wanted quite a bit more than functions. I made up a 

term "genericity" for dealing with generic behaviors in a 

quasi-algebraic form.



  - I didn't like the way Simula I or Simula 67 did inheritance 

(though I thought Nygaard and Dahl were just tremendous thinkers and 

designers). So I decided to leave out inheritance as a built-in 

feature until I understood it better.



My original experiments with this architecture were done using a 

model I adapted from van Wijngaarten's and Wirth's "Generalization of 

Algol" and Wirth's Euler. Both of these were rather LISP-like but 

with a more conventional readable syntax. I didn't understand the 

monster LISP idea of tangible metalanguage then, but got kind of 

close with ideas about extensible languages draw from various 

sources, including Irons' IMP.



The second phase of this was to finally understand LISP and then 

using this understanding to make much nicer and smaller and more 

powerful and more late bound understructures. Dave Fisher's thesis 

was done in "McCarthy" style and his ideas about extensible control 

structures were very helpful. Another big influence at this time was 

Carl Hewitt's PLANNER (which has never gotten the recognition it 

deserves, given how well and how earlier it was able to anticipate 

Prolog).



The original Smalltalk at Xerox PARC came out of the above. The 

subsequent Smalltalk's are complained about in the end of the History 

chapter: they backslid towards Simula and did not replace the 

extension mechanisms with safer ones that were anywhere near as 

useful.



>

>     What does "object-oriented [programming]" mean to you?

>     (No tutorial-like introduction is needed, just a short

>     explanation [like "programming with inheritance,

>     polymorphism and encapsulation"] in terms of other concepts

>     for a reader familiar with them, if possible. Also, it is

>     not neccessary to explain "object", because I already have

>     sources with your explanation of "object" from

>     "Early History of Smalltalk".)



(I'm not against types, but I don't know of any type systems that 

aren't a complete pain, so I still like dynamic typing.)



OOP to me means only messaging, local retention and protection and 

hiding of state-process, and extreme late-binding of all things. It 

can be done in Smalltalk and in LISP. There are possibly other 

systems in which this is possible, but I'm not aware of them.



Cheers,



Alan



>

>   Thank you,

>

>   Stefan Ram
