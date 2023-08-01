# Reading 14

## Intro to password hashing

Define the term “hashing”.

To chop up into small pieces, in this case its our password we want to hash will only have one way encryption.

Explain to a non-technical friend what a hash function does to a password.

Think about tapping cards to purchase things at the groceries instead of entering your pin after a swipe. You don't have to put in you pin (password) the card puts out radio frequencies that are probably hashed. With the radio waves, there likely isn't a way to get your pin.

## bcrypt overview

What does it mean to ‘salt’ a password?

Seems like its another element that gets mixed with the password before being hashed. I think similar to the concept of 2 factor auth. You need both password and the salt to get it cracked

What piece of information would a hacker need to access in order to find the ‘salt’ string for your passwords?

The "salt" string is not meant to be kept secret; it's stored alongside the hashed passwords in the database. The idea is that each user has their own unique salt, so if an attacker gains access to the password hashes, they would also have access to the corresponding salts. However, this is not a security concern because the salt is only useful in combination with the user's password.

## jBCrypt (the paragraphs and code example at the top of the page)

How does the Blowfish block cipher handle the increased computation speed of new computers?

With increasing sppeds of new computers Blowfish can increase the size of keys it can use. Blowfish can efficiently handle key sizes from 32 bits up to 448 bits. To maintain security and slow down brute-force attacks, you can simply increase the key size used in the Blowfish cipher.

What are the issue with the two most common password hashes for Java (“Java password hash” and “Java password encryption”)?

<!-- CHATGPT HELPED WITH THIS QUESTION -->

Java Password Hash: Developers used simple and insecure methods to hash passwords, like using the String.hashCode() function. However, this method is not suitable for password hashing because it lacks cryptographic strength and is susceptible to brute-force attacks.

Java Password Encryption: Encryption is a reversible process, meaning encrypted data can be decrypted back to its original form. For password storage, you want a one-way function (like a hash) that is non-reversible. If passwords are encrypted and the decryption key is compromised, attackers can easily obtain the original passwords.

## Things I want to know more about

## References

[Intro to password hashing](https://auth0.com/blog/hashing-passwords-one-way-road-to-security/)

[bcrypt overview](https://danboterhoven.medium.com/why-you-should-use-bcrypt-to-hash-passwords-af330100b861)

[jBCrypt](https://www.mindrot.org/projects/jBCrypt/)
