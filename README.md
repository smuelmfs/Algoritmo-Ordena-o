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

## Otimizar o desempenho do MergeSort, quando a instância for muito pequena, ele deverá chamar o InsertionSort no lugar da recursão.

Para poder chamar o InsertionSort no MergeSort, foi necessário realizar a sobrecarga no InsertionSort para que o mesmo passasse a permitir a passagem de parâmetros:

```
    public void sort(int[] A){
        int key;
        for (int j = 1; j < A.length; j++) {
            key  = A[j];
            int i = j - 1;
            while ((i > 0) && (A[i] > key)){
                A[i + 1] = A[i];
                i --;
            }
            A[i + 1] = key;
        }
    }
```

E então, com a condicional abaixo, é decidido se o retorno será via o próprio MergeSort, ou, se será chamado o InsertionSort.

```
   public void sort ( int p, int r){
        int q;

        //Adcionado if para validar considerando a instancia pequena como até 1000.
        //Se a instancia for até 1000, chama-se o InsertionSort no lugar do MergeSort.

        if (A.length <= 1000){
            insertionSort.otimizandoSort(A);
        }
        //Senão, se a instancia for maior que 1000, chama-se o próprio MergeSort recursivo.
        else {
            if (p < r) {
                q = Math.floorDiv((p + r), 2);
                sort(p, q);
                sort(q + 1, r);
                merge(p, q, r);
            }
        }
    }
```

## Conclusão:

InsertionSort é mais apropriado ao lidar com pequenas quantidades de dados, especialmente quando os dados provavelmente serão classificados ou parcialmente classificados.
MergeSort é melhor para grandes quantidades de dados classificados aleatoriamente ou em ordem decrescente. Dados o seu dividir e conquistar, os dados já ordenados demoram mais neste algoritmo, o que vai atrapalhar os dados (devido ao fato da divisão) e ter que ordená-los novamente.
BubbleSort faz um loop sobre o vetor várias vezes, colocando o maior elemento da sequência no topo a cada vez. Por ter que passar pelo vetor várias vezes, é final em todos os testes executados.

---
