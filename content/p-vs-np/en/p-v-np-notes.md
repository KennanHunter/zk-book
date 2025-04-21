P v NP v PSPACE

I've always learned PSPACE programs are called EXP problems, i should look into what the differences in notation might mean

"PSPACE Example 1: Finding the optimal Chess move" My first thought is that you can still use heuristics to make good guesses of validity, like if it's the best move in a resource value/resource location heuristic then you get a pretty good view of if the powerful computer actually did the math, is there a formalization of this? Perhaps something along the lines of how concrete said heuristic would have to be to properly validate if the computer completed it even without a proper "witness"

"PSPACE Example 2: Determining if regexes (regular expressions) are equivalent" 
i trust that it actually is a super hard PSPACE problem but i remember Cloudflare was doing some cool graph representation stuff of regexes and i always thought that there was *probably* some way of collapsing equivalent regexes into equivalent graphs, using some order of operations algebra style, it's a interesting thing to think about

I really like this graph, may update it at some point

| Category | Compute Time                 | Verification Time            |
| -------- | ---------------------------- | ---------------------------- |
| P        | Must be polynomial or better | Must be polynomial or better |
| NP       | No Requirement               | Must be polynomial or better |
| PSPACE   | No Requirement               | No Requirement               |

It took a minute but i follow the p vs np for the boolean >= op, how this extends to like real problems i do not get

> Thus, we see that a witness that proves a list is sorted does not have to be the sorted list. It can also be the input to Boolean formula that we created above that results in the formula returning true.

~~okay... so how do we use this to actually make verifying faster~~ edit: ahh "Being able to convert any problem into a Boolean formula is not a cheat code for finding the answer efficiently."

interesting that the 3 color boundary has it's expression count grow exp.

> However, for any heuristics designed to speed up solving an NP problem, it is possible to create a pathological instance of problem that is designed to exploit the heuristic and make it worthless

This sounds like fun to do 


# Conclusion

Using the solve/verify definition, P problems are verified and solved both in polynomial time, typically meaning the fastest way to verify is to simply solve, while NP problems are verified in polynomial time but solved in exponential time. PSPACE problems are those that are verified and solved in polynomial time 

Converting a problem to it's binary circuit form is a generalized method for creating a single Boolean equation that describes a problem such as to be used in the verify part of the solve/verify definition of a NP class problem 

# Open questions

Is the fact that P problems are verified and solved both in polynomial time a generalization or a identity?

I still don't have the different classes 100% commited, perhaps because I struggle to remember things that I can't tie into their importance/application.  

How do we do this with arithmetic circuits?