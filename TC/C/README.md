﻿
Problema H

Execução de uma maquina de Turing

Problema

O objectivo deste exerccio e a implementac~ao do processo de execuc~ao de maquinas de Turing, como descrito nos apontamentos das aulas da disciplina. Vamos nos limitar neste exerccio ao caso das execuc~oes que terminam em tempo razoavel. Uma execuc~ao e razoavel quando termina em menos do que 200 passos.

Input

O input introduz o valor inicial da ta e a denic~ao da maquina de Turing M = (Q;  ;; ;s;];F). Para simplicar o formatos dos dados em entrada admitiremos aqui que o conjunto dos estados Q

e sempre da forma f1:::ng (n inteiro), que  = fa;:::;zg, que   = f];A;B;:::;Z g [  e que o estado inicial e o estado 1.

Na primeira linha e introduzida a palavra por reconhecer. Esta palavra so e constituida por caracter do alfabeto  tem por comprimento maximo 50 caracteres.

Nas linhas restantes s~ao introduzidos os dados necessarios a denic~ao completa da maquina de Turing M.

Assim M = (Q;  ;; ;s;];F) e introduzida por:

- uma linha com o inteiro n, especi cando o conjunto Q = f1:::ng;
- uma linha com o numero nf (cardinalidade do conjunto F dos estados nais);
- uma linha com nf inteiros distintos (separados por um espaco) que formam o conjunto dos estados nais;
- uma linha com o numero m de transic~oes (a cardinalidade de ));
- m linhas em que cada uma delas introduz uma transi c~ao sob a forma de i a b d j, i sendo o inteiro representando o estado de partida da transic~ao, a o caracter no rotulo da transic~ao, bo caracter por escrever na ta, d 2 fL;Rg a direcc~ao do movimento da cabeca de leitura/ecrita

e j o inteiro que representa o estado de chegada

Output

Dois casos: ou a execuc~ao decorreu e terminou em menos do que 200 passos ( 200) ou n~ao.

1. No primeiro caso o input e constituido por tr^es linhas. Seja (s; ; ) a congurac~ao nal. Se

s e nal ent~ao a primeira linha contem a palavra YES, sen~ao a palavra NO.

A segunda linha apresenta o conteudo da ta, ou seja esta linha apresenta a palavra . Relembramos que  e a palavra vazia e como tal e o elemento neutro da concatenac~ao.

A terceira linha apresenta um inteiro. Este inteiro e o numero total de passos que a execuc~ao necessitou para terminar.

2. No segundo caso a resposta deve ser uma unica linha com o conteudo: DON'T KNOW

**Sample Input**
```
aaabbb
5
1
5
10
1 a X R 2 
1 Y Y R 4 
2 a a R 2 
2 b Y L 3 
2 Y Y R 2 
3 a a L 3 
3 X X R 1 
3 Y Y L 3 
4 Y Y R 4 
4 # # R 5
```
**Sample Output**
```
YES 
XXXYYY# 
25
```