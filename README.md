# Hashcat

Cracking passwords has many legitimate uses, besides the obvious criminal and espionage ones. A sysadmin may wish to pre-emptively check the security of user passwords. If Hashcat can crack them, so can an attacker.

To install 
sudo apt update
sudo apt-get install hashcat


to open sudo hashcat

 # | Mode
 ===+======
  0 | Straight
  1 | Combination
  3 | Brute-force
  6 | Hybrid Wordlist + Mask
  7 | Hybrid Mask + Wordlist
  9 | Association

 ? | Charset
 ===+=========
  l | abcdefghijklmnopqrstuvwxyz [a-z]
  u | ABCDEFGHIJKLMNOPQRSTUVWXYZ [A-Z]
  d | 0123456789                 [0-9]
  h | 0123456789abcdef           [0-9a-f]
  H | 0123456789ABCDEF           [0-9A-F]
  s |  !"#$%&'()*+,-./:;<=>?@[\]^_`{|}~
  a | ?l?u?d?s

 # | Device Type
 ===+=============
  1 | CPU
  2 | GPU
  3 | FPGA, DSP, Co-Processor

- [ Workload Profiles ] -

  # | Performance | Runtime | Power Consumption | Desktop Impact
 ===+=============+=========+===================+=================
  1 | Low         |   2 ms  | Low               | Minimal
  2 | Default     |  12 ms  | Economic          | Noticeable
  3 | High        |  96 ms  | High              | Unresponsive
  4 | Nightmare   | 480 ms  | Insane            | Headless


	Hashcat-data
Hashcat is an advanced CPU/GPU-based password recovery utility supporting seven unique modes of attack for over 100 optimized hashing algorithms.

to do that 
sudo apt install hashcat-data

3.1.2	Password Lists In Kali
Kali comes pre-packaged with wordlists that can be used for cracking passwords. The wordlist files are in the /usr/share/wordlists directory.
The one that is used the most, especially when doing a CTF (capture the flag), is the rockyou.txt file. This file is massive, It contains over fourteen million user passwords.


pip install hashid
Once installed, you simply type hashid -m and the hash you need to be identified, as seen below. This will show the corresponding Hashcat mode alongside the potential hash. Let’s take the following hash and put it into hashID

