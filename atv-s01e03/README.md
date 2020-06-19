# Tipos de Sistema Distribuidos

## Sistema de Computação Distribuidos :computer: :heavy_minus_sign: :computer:
 
  Foco em desempenho, grandes processamentos a exemplo do que foi feito na renderização da primeira imagem de um buraco negro.

  - Compartilhamento de Recursos 
  - Abertura :unlock:
  - Concorrência
  - Escalabilidade
  - Tolerância a Falhas
  - Transparência :eyeglasses:
  
  ACID, Característica importante para os sistemas distribuidos. 1.Atomicidade, 2.Consistência, 3.Isolamento e 4.Durabilidade
  1. Todas operações tem um destino binário (Sucesso ou Falha)
  2. Não violar invariantes do Sistema, dados sensíveis devem ser preservados, casos de transações, agendamento, etc.
  3. Uma operação não interfere em outra, porém todas devem ser executadas em ordem. Mantendo a distinção entre elas
  4. Depois de confirmados as modificações, devem ser mantidas ate que seja necessário alterar. 

### Computação em Cluster
- Conectados através de uma LAN
- Homogêneos
- Único nó de Gerenciamento

### Computação em grade
- Heterogêneos
- Conectados atraves de WAN

### Pervasívos
 Algumas características relevantes são:
 - Ciência de Contexto, diz respeito as condições do ambiente naquele momento. Ex: Qualidade da Internet ou Resolução da Câmera, depende de cada cliente, é necessário atender a todos.
 - Heterogeneidade de rede e de dispositivos, comum em sistemas feitos para performar em vários dispositivos atualmente, como os navegadores, apps.
 - Uso de Baterias, comum nos dispositivos mais recentes
 - Interface com o Usuário
 - Problemas de segurança, é suscetível a falhar devido a variedade de dispositivos

 ### Redes de Sensores Sem Fio

    Uma rede de sensores que monitoram determinado ambiente e compartilham de um mesmo nó para onde os dados são enviados e processados
 > Essa é uma das redes que tende a se popularizar ainda mais com a chegada do 5G e uso de tecnologias IoT

 ## Midleware

 > Camada intermediária que está entre o SO e as Aplicações Distribuidas.

 Vai evitar a implementação de baixo nível para os dispositivos, agilizando o processo e abstraindo alguns passos mais trabalhosos.

 - Facilidade de comunicação
 - Nomeação
 - Persistência 
 - Transações Distribuidas
 - Segurança
> Midwares Abertos compartilham os mesmos protocolos e interfaces