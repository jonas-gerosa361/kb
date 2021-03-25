# Monolito
** Modelo mais simples e normalmente mais utilizado. Algo que acontece muito é um sistema começar como monilito e ao crescer ter a necessidade de migrar para microserviço **
Neste modelo a aplicação é criada inteira em cima de um servidor ou node, onde se houver uma alta demanda podemos ter downtime de uma aplicação.

## Pros
* Baixa complexidade
* Monitoramento simplicado

## Contras
* Stack única
* Compartilhamento de recursos
* Acoplamento
* Mais complexo para escalar

# Microserviços #1
** Modelo mais complexo mas considerado muito mais efetivo do que monolito **
Neste modelo, um sistema é quebrado em serviços que não necessariamente dependem de si.

## Pros
* Stack dinâmica (não fico preso há uma linguaguem)
* Simples para escalar

## Contras
* Acoplamento
* Monitoramento mais complexo
* Provisionamento mais complexo

# Microserviços #2
** Modelo muito parecido com o modelo 1, porém para comunicação entre os serviços é feita utilizado um broker **

## Pros
* Stack dinâmica
* Simples para escalar
* Desacoplamento

# Contras
* Monitoramento mais complexo
* Provisionamento mais complexo

# Microserviços #3
** Modelo que utiliza um gerenciador de pipeline para decidir qual serviço será utilizado e qual será o próximo serviço **

## Pros
* Stack dinâmica
* Simples escalabilidade
* Desacoplamento
* Menor complexidade

## Contras
* Provisionamento mais complexo
* Plataforma inteira depende do gerenciador de pipeline (Single Point of Failure?)

# Gerenciamento de erros

## Maiores complexidades
* processos assincronos (Microserviços #2)
* Pipeline (Microserviço #3) - necessidade de fazer rollback em casos de erros (nem sempre é possível)

## Solução
* Dead letter queue
* Filas de re-tentativas