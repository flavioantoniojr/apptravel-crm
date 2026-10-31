# AppTravel Group · visão integrada (app do grupo + CRM da agência)

Protótipo navegável que mostra os dois lados ao mesmo tempo:

- **à esquerda, o CRM da agência**, no computador;
- **à direita, o celular do grupo**, no app.

O que um lado faz aparece no outro na hora. A base são as regras decididas em 31/10/2026 ([integração app ↔ CRM](https://github.com/flavioantoniojr/apptravel_group/blob/main/ideacao/integracao-app-crm.md), seção 0; repositório privado).

## As três personas

| Persona | Onde age | O que faz |
|---|---|---|
| **Flávio Rodrigues**, cabeça do grupo | Celular | Escolhe a agência, autoriza por todos, aceita a proposta, avalia e pede a próxima viagem |
| **Marta Rodrigues**, membro do grupo | Celular | Responde ao orçamento, reage à proposta item a item, acompanha e avalia |
| **Ana Souza**, dona da agência | CRM | Recebe o lead, aceita, faz o contato, monta a proposta, compra os itens e lança despesas |

Acima do celular há uma chave para trocar entre o Flávio e a Marta.

## Como validar (12 passos)

O painel da direita mostra o passo atual, **quem age** e o botão **Ir para este passo**. Cada passo se marca sozinho quando é feito.

1. **Marta:** responde às duas perguntas de orçamento (por dia no destino e viagem inteira). O app avisa que a agência escolhida verá as respostas.
2. **Flávio:** escolhe a agência numa lista ordenada pelo score, autoriza por todos e envia. As escolhas travam.
3. **Ana:** recebe o aviso no sininho e abre o lead. Vê uma prévia sem nomes nem contatos e tem 1 dia útil para decidir.
4. **Ana:** aceita o lead. Aparecem o nome e o contato de todos, e o grupo vê no celular quem vai atender e até quando.
5. **Ana:** marca "contato feito" depois de falar com o Flávio pelos canais dela.
6. **Ana:** monta a proposta a partir do roteiro e envia pelo app. Também pode enviar por fora e marcar o ganho informando o valor.
7. **Marta:** reage à proposta item a item (👍 ou "trocaria").
8. **Flávio:** vê o que o grupo achou e aceita. O negócio vai para "ganho" no CRM.
9. **Ana:** cria a viagem e compra os itens. Cada compra chega ao celular com status, voucher e valor.
10. **Ana:** lança uma despesa para o grupo, que aparece no app só para ver.
11. **Marta:** no dia seguinte à volta, avalia a agência. A avaliação não depende de acertar as contas.
12. **Flávio:** com a nota do grupo em 4 ou mais, a próxima viagem volta para a mesma agência.

**Desvio que também dá para testar:** no passo 3 ou 4, clique em **Recusar**. O lead segue para a próxima agência pelo score, e o Flávio é avisado.

Para recomeçar, use **Reiniciar protótipo**, no rodapé do menu.

## O que é simulado

- **Todos os nomes, valores, hotéis e companhias aéreas são de exemplo.**
- Lúcia e Pedro não reagem nem avaliam: o protótipo só mostra o Flávio e a Marta.
- Não funcionam:
  - busca e filtros;
  - o "Criar" manual;
  - escolher a Agência B ou C;
  - "Seguir sem agência";
  - desistir do pedido;
  - negociação perdida.

  As regras de cada um estão descritas nos avisos do protótipo e no documento de integração.
- A cobrança da agência acontece por fora e não aparece para o grupo.
- O modelo de cobrança das agências (assinatura) está em estudo e não aparece no protótipo.
- Nada é salvo: recarregar a página volta ao início.

## Arquivos

- `index.html`: o protótipo inteiro (HTML, CSS e JavaScript, sem dependências).
- `assets/emo.js`: ícones 3D (Microsoft Fluent Emoji, licença MIT).
- `assets/fotos.js`: fotos do Wikimedia Commons; créditos no repositório do [protótipo do app](https://github.com/flavioantoniojr/apptravel-prototipo/blob/main/creditos-fotos.md).
