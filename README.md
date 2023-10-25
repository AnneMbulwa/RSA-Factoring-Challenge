/*RSA factoring challenge*/
RSA is the most widely used public-key cryptography algorithm in the world
- It is also one of the most secure, with only a few known attacks that can be used to break it. but this is by design and not by accident.
- The RSA algorithm is a public-key cryptosystem. This means that there are two keys, a public key, and a private key. 
- The public key can be known by everyone and is used for encryption.
- The private key is known only by the owner and is used for decryption.
- The RSA algorithm is asymmetric, which means that the encryption and decryption keys are different.

RSA was developed in the 1970s by Ron Rivest, Adi Shamir, and Len Adleman. It is based on the difficulty of factoring large numbers.
- The RSA algorithm is based on the fact that it is very difficult to factorize large numbers.
- The security of the RSA algorithm, therefore, depends on the fact that the factorization of large numbers is a difficult problem.

NOTE
 /*To encrypt a message, each letter in the message is converted into a number using a scheme such as ASCII.
Then, for each number, it is raised to the encryption key power and divided by the modulus.
The remainder of this division is the encrypted number. To decrypt a message, each encrypted number is raised to the decryption key power and divided by the modulus.
The remainder of this division is the decrypted number.
This number is then converted back into a letter using the same scheme as before.*/

RSA has variety of applications, including email, file sharing, and secure communications.
It is also used in many different protocols, such as SSL/TLS, which is used to secure communications on the Internet.

RSA also has a weakness and that is vulnerable to attack if the private key is compromised.
Another weakness is  it is relatively slow compared to other public-key algorithms.

Steps to how RSA works:
1. Select the two distinct prime numbers, p and q.
Compute n = pq.
Compute the Euler's totient function, φ(n) = (p-1)(q-1).
Select an integer, e, such that 1 < e < φ(n) and gcd(e, φ(n)) = 1.
Calculate the modular multiplicative inverse of e modulo φ(n), denoted as d.
The public key consists of the pair (e, n), and the private key consists of the pair (d, n). 

2. encrypt message:
	c = m^e mod n
	where: c is the ciphertext and m is the message we want to encrypt.

3. decrypt message:
		m = c^d mod n
		where: m is the decrypted message

note::
	Note that m = message (that will be converted to an integer with padding)

/*Prime Factorization*/
Prime factorization is a process of decomposing a given composite number into its prime factors.
