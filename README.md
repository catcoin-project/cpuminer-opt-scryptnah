# cpuminer-opt-scryptnah
JayDDee's cpuminer-opt compiled to support scrypt-nah for Strayacoin.

# Virus scanner false positives
All mining programs are automatically flagged as threats.  cpuminer-opt is not a virus, backdoor or anything else malicious; you will have to add an exception for it like all other mining programs.

# Use at a Straycoin pool that supports scrypt-NAH
Currently, the only mining pool that supports scrypt-NAH that I am aware of is my own, at https://pool.larahelpers.com.

Mining pools have to modify their stratum server code to support scrypt-NAH.  The pool at larahelpers.com (despite saying scrypt) actually tests for scrypt-NAH hashes.

Point your miner there with:
```
cpuminer.exe -a scrypt -u <your wallet address> --hash-meter -o stratum+tcp://pool.larahelpers.com:3433 -p c=NAH
```
