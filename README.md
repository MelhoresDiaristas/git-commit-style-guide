# Melhores Diaristas Padrão de Mensagens de Commit

### Introdução

Este guia tem a finalidade de propor um padrão para as mensagens de commit nos 
projetos do [Melhores Diaristas](https://www.melhoresdiaristas.com.br).

É fortemente baseado (pra não dizer tradução livre) nos guias de estilo de 
commits utilizados em grandes projetos opensource, incluindo o Linux Kernel.

A padronização, além do benefício de unificar o estilo entre as equipes e 
projetos, tende a permitir a visualização do histórico como se fosse um 
**CHANGELOG** vivo, que é atualizado automaticamente a cada novo commit.

### Mensagens de Commit

##### Estrutura

Uma mensagem de commit consiste de três partes distintas, separadas 
obrigatoriamente por uma linha em branco: um **título** *(obrigatório)*, um 
**corpo** *(opicional)* e um **rodapé** *(opicional)*. 

```
tipo: assunto

corpo

rodapé
```

##### Tipos

- **feat**: Implementação de alguma novidade: Uma feature, funcionalidade, tela, 
opção de ação, etc.
- **fix**: Implementação em que a única finalidade é corrigir algum comportamente 
errôneo do sistema.
- **docs**: Alterações ou incrementos na documentação do projeto.
- **style**: Refatorações de identação, vírgulas ausentes, otimização de imports 
e etc.
- **refactor**: Refatoração/melhoria de código sem alterar funcionalidade.
- **test**: Refatoração ou adição de testes. Apenas testes.
- **chore**: Alterações em arquivos de configuração do projeto ou do ambiente. 
Logs, pacotes, dependências e etc.


##### Assunto

Assuntos não devem conter mais do que 50 caracteres, devem começar com uma 
letra maiúscula e não devem ter um ponto final.

Use um tom imperativo para descrever o que um commit faz, ao invés de o que 
ele fez.

##### Corpo

Nem todos os commits são suficientemente complexos para necessitar de um corpo.
Você pode deixar de incluir o corpo em casos em que seja possível deixar clara 
a intenção do commit apenas com o título.

Quando necessário, use o corpo do commit para explicar o que foi feito e por
qual motivo. 

Nunca use o corpo do commit para dizer "como" foi feito.

##### Rodapé

O rodapé deve ser utilizado quando for necessário se referir a IDs de sistemas
de gerenciamento de bugs e tarefas.

##### Exemplo de mensagem de commit

```
feat: Disponibiliza opcao de pedir servico de passadoria de roupas

Disponibilizada no site a funcionalidade de criar um novo pedido do tipo
Passadoria de Roupas, com as seguintes opcoes:

- 4 horas
- 6 horas
- 8 horoas

Tarefa: #123
Ver também: #456, #789
```
