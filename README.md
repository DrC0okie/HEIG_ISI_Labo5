# HEIG_ISI_Labo5
Attaques logicielles:  Manipulations Mémoire

## Quesiton 3.1
> x=2


## Question 3.2:
instruction : add    DWORD PTR [rbp-0x4],0x1
Adresse: main()+35

## Question 3.3:
Instruction: add    DWORD PTR [rbp-0x4],0x1
Adresse main()+39

## Question 3.4:
Instruction complète: 

cout << "x=" << x << endl;

> affichage de "x="

```
main()+43: lea    rax,[rip+0xe25]        # 0x555555556004
main()+50: mov    rsi,rax
main()+53: lea    rax,[rip+0x2e97]        # 0x555555558080 <_ZSt4cout@GLIBCXX_3.4>
main()+60: mov    rdi,rax
main()+63: call   0x555555555040 <_ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@plt>
```

> affichage de la variable x

```
main()+68: mov    rdx,rax
main()+71: mov    eax,DWORD PTR [rbp-0x4]
main()+74: mov    esi,eax
main()+76: mov    rdi,rdx
main()+79: call   0x555555555070 <_ZNSolsEi@plt>
```

> Retour à la ligne

```
main()+84: mov    rdx,QWORD PTR [rip+0x2dc8]        # 0x555555557fd0
main()+91: mov    rsi,rdx
main()+94: mov    rdi,rax
main()+97: call   0x555555555050 <_ZNSolsEPFRSoS_E@plt>
```

## Question 3.5

### Adresse de base du main :

```
0x00005555555551ad
```


### Adresse relative de la première incrémentation de x :

```
main()+35 -> = main()+0x23
```

### Adresse absolue de la première incrémentation de x :

```
0x00005555555551ad + 0x23 = 0x00005555555551d0 
```

## Question 3.6

###  Adresse relative de la deuxième incrémentation de x :

```
main()+39 -> = main()+0x27
```

### Adresse absolue de la deuxième incrémentation de x :

```
0x00005555555551ad + 0x27 = 0x00005555555551d4 
```


## Question 3.7 

```
43 = 0x2b
0x00005555555551ad + 0x28 = 0x00005555555551d8
```
## Question 3.15

En accédant à la variablle classe[7] nous accédons enfaite à la variable grade[3], la variable n'étant pas initialisé sa valeur initial était 21845 et donc sa valeur après l'éxécution de l'instruction classe[7] est de 21855

(ajouter schéma)
