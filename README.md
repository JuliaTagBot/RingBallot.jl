# RingBallot.jl

Let's assume a linkable ring signature scheme. Then a following electronic ballot system can be constructed:

1. Members connect to the server and verify their identity
2. The server waits for multiple members and sends to everyone participating member public keys. 
3. Each member makes a ring signature for his vote. 
4. The member sends the signature and the vote anonymously to the ballot receiving port.
5. The server verifies all received votes and publishes the ballot if successful.

# Comments

+ The security of a linkable ring scheme can be doubted on the grounds of its novelty and a lack of widespread use.
+ Anonymous network is necessary to send the votes.
+ One participating member can sabotage the process anonymously by not sending the vote.
+ The server and internet service provider can implement a timing attack to deanonymise the votes.
