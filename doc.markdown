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

Livro [Operating Systems for Supercomputers and High Performance Computing](https://link.springer.com/book/10.1007/978-981-13-6624-6)

Artigos:
* [The Multikernel: A new OS architecture for scalable multicore systems](https://barrelfish.org/publications/barrelfish_sosp09.pdf)
* [A Multi-Kernel Survey for High-Performance Computing](https://dl.acm.org/doi/10.1145/2931088.2931092)

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
  * [slides](https://www.sandia.gov/app/uploads/sites/210/2022/11/pedretti_lanl11.pdf) sobre o kernel
* [McKernel](https://github.com/RIKEN-SysSoft/mckernel)
* [mOS](https://github.com/intel/mOS)
  *  Um fork do Linux feito pela intel para HPC.
  *  Multi-kernel
  *  Alguns artigos sobre:
    *  [Sua arquitetura](https://dl.acm.org/doi/10.1145/2612262.2612263)
    *  [Avaliação de desempenho](https://ieeexplore.ieee.org/document/8425166)
    *  [Integrando containers ao mOS](https://dl.acm.org/doi/10.1145/3095770.3095777)
    *  [Poster](https://www.researchgate.net/publication/338659991_Multi-OS_for_HPC_Fact_Sheet)
* [Barrelfish](https://barrelfish.org/):
  * Feito pela ETH Zurich e Microsoft R&D

## DevOps e engenharia de plataforma para HPC

A ideia é propor as práticas de DevOps e engenharia de plataforma para o ambiente acadêmico.

* Artigo: [Continuous Integration and Delivery for HPC: Using Singularity and Jenkins](https://dl.acm.org/doi/10.1145/3219104.3219147)
* Artigo: [Continuous Integration for HPC with Github Actions and Tapis](https://dl.acm.org/doi/10.1145/3491418.3535124)
* Artigo: [Singularity: Scientific containers for mobility of compute](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0177459)
* Artigo: [Containers in HPC: a survey](https://dl.acm.org/doi/10.1007/s11227-022-04848-y)
* Artigo: [Containerization for High Performance Computing Systems: Survey and Prospects](https://dl.acm.org/doi/10.1109/TSE.2022.3229221)
* Artigo [Shifter: Containers for HPC](https://cug.org/proceedings/cug2016_proceedings/includes/files/pap103s2-file1.pdf)
