# HEIG_ISI_Labo5
Attaques logicielles:  Manipulations Mémoire

## Quesiton 3.1
> x=2


Question 3.2:
instruction : add    DWORD PTR [rbp-0x4],0x1
Adresse: main()+35

Question 3.3:
Instruction: add    DWORD PTR [rbp-0x4],0x1
Adresse main()+39

Question 3.4:
Instruction complète:

main()+43: lea    rax,[rip+0xe25]        # 0x555555556004
main()+50: mov    rsi,rax
main()+53: lea    rax,[rip+0x2e97]        # 0x555555558080 <_ZSt4cout@GLIBCXX_3.4>
main()+60: mov    rdi,rax
main()+63: call   0x555555555040 <_ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@plt>
main()+68: mov    rdx,rax
main()+71: mov    eax,DWORD PTR [rbp-0x4]
main()+74: mov    esi,eax
main()+76: mov    rdi,rdx
main()+79: call   0x555555555070 <_ZNSolsEi@plt>
main()+84: mov    rdx,QWORD PTR [rip+0x2dc8]        # 0x555555557fd0
main()+91: mov    rsi,rdx
main()+94: mov    rdi,rax
main()+97: call   0x555555555050 <_ZNSolsEPFRSoS_E@plt>