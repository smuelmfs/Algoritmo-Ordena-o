```
Aluno: Samuel Messias
RA: 12012827

```

# Comparação de Desempenho

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
