CE5_Sisco
=========

##Task 1 and 2

------------
\\$S0 = 44


\\$S1 = -37


Instruction code        Machine Code                            hex



addi $S0, $0, 44        00100010000000000000000000101100     0x2200002C


addi $S1, $0,-37        00100010001000001111111111011011     0x2220FFDB


add  $S2, $S0, $S1      00000010001100001001000000100000     0x02309020


sw   $S2, 84($0)        10101110010000000000000001010100     0xAE400054


##Task 3

Added the following line of code to the main decoder 


when "001101" => controls <= "101000011"; -- ori


this adds the ORI instruction capability to the machine.


Added the following line of code to the alu decoder


when "11" => alucontrol <= "001"; -- logical or (for ori)


this tells the alu to preform a logical or operation for the ori instruction
