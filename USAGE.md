# Smart Development Bridge <=2.3.2 (part of Tizen Studio 1.3 Windows x86/x64) - Buffer Overflow PoC

This code has been created for educational purposes only, to raise awareness on software security, and it's harmless
by intention (the PoC runs calc.exe). Please do not change the code behaviour to malicious

Demonstrated Exploitation Techniques:

1: Direct execution, 3-byte EIP overwrite, Stack adjustment

2: Payload for social engineering attack, JMP ESP (!mona find -s "\\xff\\xe4" -cp alphanum), Alphanumeric shellcode

3: Bonus exercise - source code analysis


### Usage: python sdbBOpoc.py [Technique_ID] [Path_to_sdb.exe] [Address_of_JMP_ESP]

Examples: python sdbBOpoc.py 1 C:\Tizen\Tools\sdb.exe

python sdbBOpoc.py 2 C:\Tizen\Tools\sdb.exe 0x76476557

python sdbBOpoc.py 3
