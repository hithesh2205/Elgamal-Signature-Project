<h1>ElGamal Signature and Forgery Attacks</h1>

<p>
This project implements the ElGamal Digital Signature Scheme and demonstrates two attacks:
</p>

<ul>
  <li>Key Reuse Attack</li>
  <li>Existential Forgery Attack</li>
</ul>

<h2>About ElGamal Signature</h2>
<p>
ElGamal is a digital signature scheme based on the discrete logarithm problem.  
It uses:
</p>

<ul>
  <li>a prime number p</li>
  <li>a generator g</li>
  <li>a private key x</li>
  <li>a public key y = g^x mod p</li>
</ul>

<p>
To sign a message, ElGamal uses a random value k.  
If k is ever reused, the private key can be recovered, breaking the system.
</p>

<h2>Attacks Implemented</h2>

<h3>1. Key Reuse Attack</h3>
<p>
If the same random k is used for two different signatures, the attacker can calculate k and then recover the private key x.
</p>

<h3>2. Existential Forgery</h3>
<p>
An attacker can create a valid signature for some message without knowing the private key by exploiting the mathematical structure of ElGamal.
</p>

