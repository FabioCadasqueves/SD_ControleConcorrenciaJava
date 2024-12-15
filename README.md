# SD_ControleConcorrenciaJava

## Arquivo Carro.java (com Semaphore):

  Utiliza um Semaphore com 10 permissões para gerenciar até 10 vagas de estacionamento simultâneas.
  Cada carro (thread) tenta ocupar uma vaga. Se todas as vagas estiverem ocupadas, a thread espera até que uma vaga seja liberada.
  O fluxo inclui aquisição de vaga (acquire), permanência (tempo aleatório) e liberação da vaga (release).
  É mais realista para simular um estacionamento com múltiplas vagas.


## Arquivo CarroLock.java (com ReentrantLock):

  Utiliza um ReentrantLock para implementar exclusão mútua.
  Apenas um carro por vez pode acessar a "vaga", o que não reflete bem um cenário com múltiplas vagas.
  O fluxo inclui aquisição do bloqueio (lock), permanência (tempo aleatório) e liberação do bloqueio (unlock).
  Serve como exemplo de uso do Lock, mas não é ideal para modelar estacionamentos.
