# 📘 Quiz de Estruturas de Dados II – Simulado


### 3. Resolução prática  
Considere uma tabela hash de tamanho **m = 7** usando o **método da divisão**.  
Calcule a posição de armazenamento das chaves: **50, 700 e 76**.  

---

### 4. Múltipla escolha  
Em uma árvore binária cheia de nível **d = 3**, o número total de nós é:  
a) 7  
b) 8  
c) 15  
d) 16  

---

### 6. Resolução prática  
Considere a expressão aritmética:  
```
a * b - (f + g) * e
```
1. Desenhe a **árvore binária** correspondente.  
2. Escreva a sequência de travessia em **pré-ordem**, **em-ordem** e **pós-ordem**.  

---

### 7. Múltipla escolha  
Sobre **Busca em Largura (BFS)**, assinale a alternativa correta:  
a) É implementada com **pilha**.  
b) Garante sempre encontrar o menor caminho entre dois vértices (em número de arestas).  
c) Tem complexidade de tempo O(n²) em todos os casos.  
d) Só pode ser usada em grafos direcionados.  

---

### 8. Raciocínio teórico  
Por que não é recomendado escolher **m** como uma potência de 2 no método da divisão para hashing?  

---


### 9. Resolução prática  
Compare os três métodos de hashing (**Divisão, Multiplicação e Dobra**) para armazenar a chave **123456** em uma tabela de tamanho **m = 100**.  
- Mostre o resultado final de cada método.  
- Discuta qual dispersa melhor e por quê.  

---

### 10. Raciocínio teórico  
Um grafo direcionado tem vértices {1,2,3,4} e arestas {(1,2), (2,3), (3,1), (3,4)}.  
- Esse grafo é **fortemente conexo**?  
- Justifique sua resposta, explicando a relação entre BFS/DFS e conectividade forte.  

---

### 11. Discursiva curta  
Explique como árvores binárias podem ser utilizadas para detectar duplicatas em uma lista de números.  
Por que esse método é mais eficiente do que comparações diretas entre todos os pares de elementos?  

---

### 12. Raciocínio teórico + prática  
(a) Explique o conceito de **corte s-t** em redes de fluxo.  
(b) Justifique por que o **Fluxo Máximo = Corte Mínimo**.  
(c) Suponha uma rede em que a capacidade de saída da origem é 7 e a capacidade de entrada do destino é 8.  
Qual é o valor máximo possível de fluxo nessa rede?  

---


📌 Questão – Fluxo em Grafos

Uma empresa de logística deseja transportar mercadorias de um armazém central (s) até um centro de distribuição (t) através de uma rede de estradas representada pelo grafo abaixo.

Cada aresta possui uma capacidade máxima de transporte (em toneladas por hora):

(s, A) = 10

(s, B) = 15

(A, C) = 9

(A, D) = 4

(B, D) = 10

(C, t) = 10

(D, t) = 15

### Perguntas:

a) Desenhe o grafo correspondente, indicando as capacidades nas arestas.

b) Determine a capacidade máxima de transporte de s até t (fluxo máximo).

c) Indique pelo menos um corte mínimo do grafo e sua capacidade.

d) Explique como o Teorema do Fluxo Máximo – Corte Mínimo garante a correção do resultado encontrado.
