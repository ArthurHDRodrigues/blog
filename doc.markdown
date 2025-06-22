---
layout: page
title: Proposta de tema para Doutorado em HPC
permalink: /doc/
---

## Metodologia para análise experimental de algoritmos em grafos

Para minha [dissertação de mestrado](https://www.teses.usp.br/teses/disponiveis/45/45134/tde-14052025-111528/en.php) implementei o algoritmo HDT para resolver o problema de conexidade em grafos dinâmicos.

Fizemos um experimento comparando com outros algoritmos seguindo [esse framework de 2022](https://www.vldb.org/pvldb/vol15/p3263-chen.pdf).
No entanto, devido a problemas de metodologia, não escrevemos um capítulo sobre isso na dissertação.

Lemos o artigo [A Theoretician’s Guide to the Experimental Analysis of Algorithms](https://web.cs.dal.ca/~eem/gradResources/A-theoreticians-guide-to-experimental-analysis-of-algorithms-2001.pdf) de David S. Johnson. Boa introdução sobre o autor: [slides](https://www.cos.ufrj.br/seminarios/2016/slides/slides_eduardo.pdf)

1. Faça experimentos dignos de nota
   Isto é; investigue questões de real interesse da comunidade.
2. Relacione seu artigo com a literatura
3. Faça testes em um conjunto de instâncias que permita se chegar a conclusões gerais
4. Projete os experimentos de forma eficiente e efetiva
5. Use implementações suficientemente eficientes
6. Garanta a reprodutibilidade
7. Garanta a comparabilidade
8. Reporte a história completa
9. Chegue a conclusões bem-justificadas
10. Apresente os dados de modo informativo


## Criar distro GNU/Linux focada em HPC

### User space
* Lembrei da apresentação: **"Ambientes computacionais para a reprodutibilidade de softwares (de pesquisa) com GNU Guix e Software Heritage"**
de maio/2024 com o Prof. Alexandre Abdo

![guix logo](./images/Guix-print(1).svg)

Guix System tem uma [equipe focada em HPC](https://hpc.guix.info/) e muitos princípios importantes para HPC:
* reprodutibilidade
* implantação de uma frota de maquinas

Outros gerenciadores de pacotes podem ser encontrados no repositório [awesome HPC](https://github.com/trevor-vincent/awesome-high-performance-computing).

### Kernel

* [Kitten](https://github.com/HobbesOSR/kitten)
  * Feito pela [Sandia labs](https://sandialabs.github.io/)
* McKernel - A hybrid kernel that combines Linux and a lightweight kernel designed to provide high performance for HPC applications.
* [mOS](https://github.com/intel/mOS)
  *  Um fork do Linux feito pela intel para HPC.
  *  Multi-kernel
  *  Alguns artigos sobre:
    *  [Sua arquitetura](https://dl.acm.org/doi/10.1145/2612262.2612263)
    *  [Avaliação de desempenho](https://ieeexplore.ieee.org/document/8425166)
    *  [Integrando containers ao mOS](https://dl.acm.org/doi/10.1145/3095770.3095777)



## DevOps para HPC
