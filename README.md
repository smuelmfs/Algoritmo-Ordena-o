```
Aluno: Samuel Messias
RA: 12012827

```

# Comparação de Desempenho:

## Modo de Comparação:

Utilizando o `System.currentTimeMillis()` foi criado uma varíavel no início e no fim do método de execução, para que assim pudessemos chegar a um valor aproximado.

Levando em consideração que o tempo de execução do algoritmo em si depende de outros fatores, como por exemplos:

- Retorno de outras Classes ` Random`.
- Capacidade de processamento da máquina.

Para chegarmos a um valor mais próximo do real possível, o algoritmo foi executado 5x em um espaço de tempo consideravél.
O resultado aproximado abaixo é a média (soma dos valores (tempo em milissegundos) dividido por 5).

---

# Avaliação de três modos diferentes:

## 1. Classe Random;

### Insertion Sort:

    - TAXA DE RESPOSTA PARA 1000 ELEMENTOS:  ≅ 3.4ms
    - TAXA DE RESPOSTA PARA 20000 ELEMENTOS:  ≅ 217.2ms

### Merge Sort:

    - TAXA DE RESPOSTA PARA 1000 ELEMENTOS:  ≅ 2ms
    - TAXA DE RESPOSTA PARA 20000 ELEMENTOS:  ≅ 9.8ms

### Bubble Sort:

    - TAXA DE RESPOSTA PARA 1000 ELEMENTOS:  ≅ 8.4ms
    - TAXA DE RESPOSTA PARA 20000 ELEMENTOS:  ≅ 919.4ms

## 2. Dados de entrada ordenados;

### Insertion Sort:

    - TAXA DE RESPOSTA PARA 1000 ELEMENTOS:  ≅ 0ms
    - TAXA DE RESPOSTA PARA 20000 ELEMENTOS:  ≅ 1.2ms

### Merge Sort:

    - TAXA DE RESPOSTA PARA 1000 ELEMENTOS:  ≅ 1.8ms
    - TAXA DE RESPOSTA PARA 20000 ELEMENTOS:  ≅ 8.2ms

### Bubble Sort:

    - TAXA DE RESPOSTA PARA 1000 ELEMENTOS:  ≅ 6.4ms
    - TAXA DE RESPOSTA PARA 20000 ELEMENTOS:  ≅ 527.8ms

## 3. Dados de entrada ordenados decrescentemente;

### Insertion Sort:

    - TAXA DE RESPOSTA PARA 1000 ELEMENTOS:  ≅ 5.6ms
    - TAXA DE RESPOSTA PARA 20000 ELEMENTOS:  ≅ 429.4ms

### Merge Sort:

    - TAXA DE RESPOSTA PARA 1000 ELEMENTOS:  ≅ 2.2ms
    - TAXA DE RESPOSTA PARA 20000 ELEMENTOS:  ≅ 9.4ms

### Bubble Sort:

    - TAXA DE RESPOSTA PARA 1000 ELEMENTOS:  ≅ 7.8ms
    - TAXA DE RESPOSTA PARA 20000 ELEMENTOS:  ≅ 552.4ms

## Conclusão:

Com o Insertion Sort as coleções com um número menor de entradas classificam um objeto por vez. No entanto, ao classificar coleções maiores, ele muda rapidamente para mergeSort, que armazena partes de cada coleção em vez de organizar cada item individualmente. A razão para isso é que a ordenação de um único dado é muito mais rápida do que a ordenação de grandes grupos. O BubbleSort gira várias vezes pelo vetor. Toda vez que ele passa, ele coloca o maior elemento no topo. Isso ocorreu porque o algoritmo precisava percorrer os dados várias vezes antes de ser o último em todos os testes.

---
