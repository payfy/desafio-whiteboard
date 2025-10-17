# Whiteboard Challenge – Sistema de Sorteios

## Contexto
Imagine que a Empresa para qual você trabalha quer lançar um sistema público de sorteios, onde qualquer pessoa possa criar e participar de sorteios online.  
Seu desafio é desenhar e explicar a arquitetura e as principais decisões técnicas para construir essa aplicação.
O foco aqui é entender como você projetaria o sistema, garantindo escalabilidade, integridade das regras e robustez diante de alta concorrência.

---

## O Problema
Precisamos de uma sistema que permita:

- Registrar usuários (nome e e-mail);
- Criar sorteios com uma data específica de execução;
- Permitir que usuários participem dos sorteios;
- Executar o sorteio automaticamente na data prevista, escolhendo um ganhador.

---

## Requisitos e Regras de Negócio
1. Impede inscrições após a data do sorteio;
2. Garante que cada usuário participe apenas uma vez em cada sorteio;
3. Lida com alta concorrência — muitos sorteios sendo criados ao mesmo tempo e sorteios muito populares recebendo milhares de inscrições simultâneas;
4. Sorteia automaticamente um ganhador na data marcada(respeitando o horario).

---

## O que é esperado que seja apresentado durante a entrevista:
- Estrutura das entidades principais (Usuário, Sorteio, Participação);
- Fluxo principal das rotas:
  - Registrar usuário  
  - Criar sorteio  
  - Participar de sorteio  
  - Consultar resultado  
- Estratégia para controle de concorrência;
- Como garantir integridade das regras mesmo sob carga alta;
- Como o sorteio é disparado na data correta;
- Estrutura básica de persistência e cache;
- Estratégia de erro e fallback.

