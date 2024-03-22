A number in binary is some finite sequence of 0 and 1 :
$$
011, 101, 1001, 0101
$$
Moreover, in all numbers, the rightmost bit which we call the elements of the sequence that can be either 0 or 1 is a 1. This is the first part of the definition the second part is that all binary sequences have a method for conversion to the decimal base.

This is guided by the following :
If the bit in the nth position in 1 then add $2^{n}$ to partial sum. Do this for all the bits to get a summation. In other words, where $a_{i} \in \{ 0, 1 \}$ and $x$ is the binary sequence $a_{0}a_{1}\dots a_{n}$ :
$$
f(x) = \sum_{i = 0}^{n} a_{i} 2^i
$$
The reason for this definition is that we want to be able to convert between all possible bases. So, by the transitive property of [[function]]s, if we can convert two bases from and to the decimal system we can simply convert to the decimal and, then, to the other base. Consequently, if all bases can be converted from and to the decimal system then all bases are convertible to each other and we have the system we were looking for.

So, the reason for this definition is so that $f^{-1}(x)$ is defined. To prove that it follows we will use the assumption of [[multiple_of_two_representation]] and that $k \in \mathbb{N}$ to argue that:
$$
k = 2m + 1 \lor k = 2m
$$
First we have to agree on the assumption that if we continuously divide by 2, we will move towards 0 so the algorithm that will be preposed must terminate.
Now if $k = 2m$ simply divide it by 2, that means we will get $m = 2m_{0} \lor m = 2m_{0} + 1$ but if $k = 2m + 1$ we may remove 1, we can do this since the first bit if active adds $2^0$. So we have two cases and once we have divided we can repeat this case again, this time because we have divided by two we know that adding a 1 is simply activating the $2^1$ bit since if we did not divide by two that one would have be multiplied by 2.

Now this process can be continued and we will gain an alternation of 0 and 1s and, thus, it would result in a representation of the decimal number. So, we have a process for doing the reverse but how do we prove that it is indeed a proper [[function]], indeed how do we even prove that $f(x)$ is a proper [[function]].

To do that we have to prove that given $x_{1} \neq x_{2} \implies f(x_{1}) \neq f(x_{2})$, this we can reason from geometric [[serie]]s, the biggest number possible if all first n bits are active is less than just the (n + 1)th bit is active. This is proved by:
$$
2^0 + 2^1 + 2^2 + 2^3 + \dots + 2^n = \frac{2^{n+1} - 2^0}{2 - 1} = 2^{n+1} - 1  
$$
But the (nth + 1) bit gives us a value of $2^{n+1}$. Thus, finishing this lemma.

Now compare two bit sequences, if one has a 1 to the right of the other then it is bigger. Consequently, we can cross those of. We continue like this from the most significant bit. Thus, if they ever don't have a 1 in the same position one will have a bit active that is right to the other and, thus, it is bigger. Which means they are not equal. As a result, they must have the same representation for the same value.

