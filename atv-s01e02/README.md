# Classificação de Hardware com várias CPUs

### Memória Compartilhada / Memória Privada -> Por barramento ou Comutador
#### Avalia o Hardware quanto a disposição de memoria para quanto aos processadores e o metodo de acesso a memória, casos de memoria privada tendem a ser mais rápidos


> O uso de barramento em memória compartilhada pode gerar o chamado gargado de Von Neumann, fazendo que a velocidade do processador seja reduzida por conta da velocidade d o barramento. 


### Multicomputadores / Multiprocessadores

#### Avaliação do Hardware quanto a: 
- Multcomputadores com cada processador e sua prórpria memória
- Multiprocessadores compatilhando uma mesma memória

### Multiprocessador em Barramento

- Cada processador possui uma memória cache interligada por barramento a memoria principal
- - Problemas Causados: Inconsistencia de cache, um ou mais processadores pode manter uma informação desatualizada a medida que são modificadas em paralelo; Limita a escalabilidade a 256 processadores
- - Vantagens: Se o cache for suficientemente grande a taxa de acerto é alta

### Multiprocessadores por Chaveamento :key:

- O chaveamento acontece através de comutadores que definem qual a vez de acessar a memória
- - Existem algumas arquiteturas para comutadores, as mais comuns são: Rede ômega e cross-bar, sendo o segundo mais custoso e inviável quando se tem um número grande de processadores. 

### Multicomputador Homogêneo

#### Aqui há uma malha de computadores com a especificação igual ou extremamente semelhante

> Traz uma ideia de cluster de computadores

### Multicomputador Heterogêneos

#### Computadores diferentes em hardware ou com software diferente, variando em diversos aspectos. 

> Um bom exemplo disso é a rede de criptomoeadas

### Taxonomia de FLynn


- SISD (Single Instruction Single Data)
- - Aqui uma instrução manipula e responde um único dado
>Todos Computadores monoprocessados entram na categoria acima

- SIMD (Single Instruction Multiple Data)
- - Um instrução gera vários dados
> Um bom exemplo SIMD são operações com Matrizes 
- MISD (Multiple Instruction Single Data)
> O cálculo da determinante de uma matriz se encaixa no MISD, pois há vários valores em uma matriz, mas o resultado é apenas um
- MIMD (Multiple Instruction Multiple Data)
> Sistemas Distribuidos normalmente se beseiam em MIMD, pois é visado processamento em massa de vários pontos do sistema 