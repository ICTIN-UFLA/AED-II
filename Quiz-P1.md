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



# 📘 Gabarito – Quiz de Estruturas de Dados II

---

### 3) Resolução prática — Tabela hash (método da divisão, m = 7)

**Fórmula:**  
\( h(k) = k \bmod m \)

- \( h(50) = 50 \bmod 7 = 1 \)  
- \( h(700) = 700 \bmod 7 = 0 \)  
- \( h(76) = 76 \bmod 7 = 6 \)

✅ **Resposta:** 50 → 1; 700 → 0; 76 → 6  

---

### 4) Múltipla escolha — Árvore binária cheia com \( d = 3 \)

Número de nós:  
\( N = 2^{(d+1)} - 1 = 2^4 - 1 = 15 \).

✅ **Alternativa correta:** c) 15  

---

### 6) Resolução prática — Árvore de expressão e percursos

Expressão:  
```
a * b - (f + g) * e
```

**Árvore da expressão:**
```
           (-)
          /   \
        (*)    (*)
       /  \    /  \
      a    b  (+)  e
             /   \
            f     g
```

- **Pré-ordem:** `-  *  a  b  *  +  f  g  e`  
- **Em-ordem:** `a  *  b  -  f  +  g  *  e`  
- **Pós-ordem:** `a  b  *  f  g  +  e  *  -`  

---

### 7) Múltipla escolha — BFS

✅ **Alternativa correta:** b)  
> BFS garante encontrar o menor caminho entre dois vértices em número de arestas (em grafos não ponderados).

---

### 8) Raciocínio teórico — Hashing com potência de 2

Não se recomenda \( m = 2^p \) porque o cálculo \( k \bmod 2^p \) usa **apenas os bits menos significativos** de \( k \).  
Isso reduz a dispersão e aumenta colisões quando as chaves compartilham padrões nesses bits.  
Por isso, costuma-se escolher \( m \) **primo** ou não potência de 2.

---

### 9) Resolução prática — Comparação de métodos de hashing  
Chave: **123456**, \( m = 100 \).

1. **Divisão:** \( 123456 \bmod 100 = 56 \).  
2. **Multiplicação (A ≈ 0,618...):** \( h = 0 \).  
3. **Dobra (12 + 34 + 56 = 102):** \( 102 \bmod 100 = 2 \).

✅ **Resultados:**  
- Divisão → 56  
- Multiplicação → 0  
- Dobra → 2  

**Discussão:**  
- Divisão depende só dos dígitos finais.  
- Dobra usa mais dígitos, mas pode concentrar padrões.  
- Multiplicação tende a dispersar melhor, pois usa a parte fracionária de \( kA \).

---

### 10) Raciocínio teórico — Grafo direcionado

Vértices: {1,2,3,4}, Arestas: {(1,2), (2,3), (3,1), (3,4)}  

- {1,2,3} formam ciclo (fortemente conectados).  
- O vértice 4 só é alcançado, mas não retorna.  

✅ **Resposta:** O grafo **não é fortemente conexo**.  

**Relação com BFS/DFS:** Um grafo é fortemente conexo se uma busca a partir de cada vértice alcança todos os outros (no grafo e no transposto). Aqui isso falha no vértice 4.

---

### 11) Discursiva curta — Árvores binárias e duplicatas

Inserindo cada elemento em uma **árvore de busca binária**:  
- Se o elemento já existe, é duplicata.  
- Se não existe, é inserido.  

**Complexidade:**  
- BST balanceada: \( O(n \log n) \).  
- Comparação par-a-par: \( O(n^2) \).  

✅ **Mais eficiente porque reduz o custo de busca e inserção.**

---

### 12) Fluxo em redes

**(a) Corte s-t:**  
Partição \( (S,T) \) com \( s \in S, t \in T \). A capacidade é a soma das arestas de \( S \to T \).

**(b) Teorema Max-Flow Min-Cut:**  
O valor do fluxo máximo é igual à capacidade do menor corte.

**(c) Origem = 7, destino = 8 → valor máximo possível = min(7,8) = 7.**

---

## 📌 Questão – Fluxo em Grafos (rede logística)

**Arestas:**
- (s, A) = 10  
- (s, B) = 15  
- (A, C) = 9  
- (A, D) = 4  
- (B, D) = 10  
- (C, t) = 10  
- (D, t) = 15  

### a) Grafo
Desenhar com os vértices **s, A, B, C, D, t** e capacidades acima.

### b) Fluxo máximo
Exemplo de fluxo:  
- s→A = 10, s→B = 10  
- A→C = 9, A→D = 1  
- B→D = 10  
- C→t = 9, D→t = 11  

✅ **Fluxo máximo = 20**

### c) Corte mínimo
Exemplo: \( S = \{s,B\}, T = \{A,C,D,t\} \)  
Capacidade = (s→A 10) + (B→D 10) = **20**

### d) Justificativa
Encontramos um fluxo de valor **20** e um corte de capacidade **20**.  
Pelo Teorema Max-Flow Min-Cut, o fluxo máximo é **20**, provando a correção.

---

