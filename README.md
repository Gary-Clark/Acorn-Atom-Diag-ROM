# Acorn-Atom-Diag-ROM

Quick and simple diagnostic ROM for the Acorn Atom

Program into a 4K EPROM to replace the Kernal ROM. On reset it will test the first 1k of RAM. If an error is detected, it will continually loop, addressing the same location which can then be checked with a logic analyser or a Scope.

On completion of the low ram test, it will test the VDU memory in the same manner

Then the PIA outputs are cycled in a logic pattern.

Finally the upper 5K of RAM is tested. For each 256K tested ok, a + symbol is printed. If an error is detected, the data returned and the address of the error is displayed.
![image](https://github.com/user-attachments/assets/65378ba4-fbd7-4b1a-876a-6301d65f5e96)
