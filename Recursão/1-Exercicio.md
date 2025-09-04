
# Exercícios de Algoritmos Recursivos

### 1. **Cálculo do Fatorial de um Número**
    
   O fatorial de um número \( N \) é o produto de todos os números inteiros de 1 até \( N \). Ou seja, \( N! = N 	imes (N-1) 	imes (N-2) 	imes \dots 	imes 1 \).  
   **Exemplo:** O fatorial de 5 é \( 5! = 5 	imes 4 	imes 3 	imes 2 	imes 1 = 120 \).  
   Sua tarefa é implementar um algoritmo recursivo que calcule o fatorial de um número \( N \), utilizando a fórmula recursiva:  
   \[
   fatorial(N) = N 	imes fatorial(N-1)
   \]
   O caso base ocorre quando \( N = 0 \), em que \( fatorial(0) = 1 \).

---

### 2. **Soma de Números de 1 até N**
   **Enunciado:**  
   Sua tarefa é criar um algoritmo recursivo para calcular a soma de todos os números inteiros de 1 até \( N \).  
   A soma pode ser expressa como:
   \[
   soma(N) = N + soma(N-1)
   \]
   Quando \( N \) for 0, a soma é 0, ou seja, \( soma(0) = 0 \).  
   **Exemplo:** Para \( N = 5 \), a soma seria \( 1 + 2 + 3 + 4 + 5 = 15 \).  
   O algoritmo deve continuar somando os números até atingir o caso base.

---

### 3. **Imprimir Números em Ordem Reversa**
   **Enunciado:**  
   Desenvolva um algoritmo recursivo para imprimir os números de \( N \) até 1 em ordem decrescente.  
   A ideia é começar com o número \( N \) e imprimir, em seguida, chamar a função recursivamente para imprimir \( N-1 \), até que \( N \) chegue a 0.  
   **Exemplo:** Se \( N = 5 \), a saída esperada seria:  
   ```
   5 4 3 2 1
   ```

---

### 4. **Cálculo do n-ésimo Número de Fibonacci**
   **Enunciado:**  
   A sequência de Fibonacci é formada pelos números 0 e 1, e os próximos números são a soma dos dois anteriores. Ou seja:
   \[
   fibonacci(n) = fibonacci(n-1) + fibonacci(n-2)
   \]
   O caso base ocorre quando \( n = 0 \) (fibonacci(0) = 0) ou \( n = 1 \) (fibonacci(1) = 1).  
   Sua tarefa é criar uma função recursiva que calcule o n-ésimo número da sequência de Fibonacci.  
   **Exemplo:** Para \( N = 5 \), a sequência de Fibonacci seria:
   \[
   0, 1, 1, 2, 3, 5
   \]
   O 5º número da sequência é 5.

---

### 5. **Contar o Número de Dígitos de um Número**
   **Enunciado:**  
   Crie um algoritmo recursivo para contar quantos dígitos há em um número inteiro positivo.  
   A cada vez que o número é dividido por 10, um dígito é descartado. O processo continua até que o número seja 0. O número total de divisões será o número de dígitos do número original.  
   **Exemplo:** Para o número \( 12345 \), a contagem dos dígitos é 5.  
   **Dica:** A recursão deve continuar dividindo o número por 10 até que ele seja 0, contando o número de divisões realizadas.

---
