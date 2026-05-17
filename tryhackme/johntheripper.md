## John Basic Syntax

The basic syntax of John the Ripper commands is as follows. We will cover the specific options and modifiers used as we use them.

john [options] [file path]

 - john: Invokes the John the Ripper program
 - [options]: Specifies the options you want to use
 - [file path]: The file containing the hash you’re trying to crack; if it’s in the same directory, you won’t need to name a path, just the file.

## Automatic Cracking

John has built-in features to detect what type of hash it’s being given and to select appropriate rules and formats to crack it for you; this isn’t always the best idea as it can be unreliable, but if you can’t identify what hash type you’re working with and want to try cracking it, it can be a good option! To do this, we use the following syntax:

john --wordlist=[path to wordlist] [path to file]

 - --wordlist=: Specifies using wordlist mode, reading from the file that you supply in the provided path
 -  [path to wordlist]: The path to the wordlist you’re using, as described in the previous task

Example Usage:

john --wordlist=/usr/share/wordlists/rockyou.txt hash_to_crack.txt
