# AppTravel Group · CRM da agência (protótipo)

Protótipo navegável da **Fase 2**: o CRM da agência, para computador e navegador.
Base: [especificação funcional](https://github.com/flavioantoniojr/apptravel_group/blob/main/ideacao/fase-2-crm-especificacao.md) (repositório privado).

**Objetivo:** validar com a agência a jornada completa, do lead que o grupo gera no app até a recompra.

## Como validar

1. Abra o link no computador. O painel **Roteiro de validação**, à direita, mostra 10 passos. Cada passo se marca sozinho quando você o faz, e o botão **Ir para este passo** leva até a tela certa.
2. Siga os 10 passos:
   1. Ver o novo lead no início.
   2. Abrir o lead Roma e Florença (grupo, orçamento por pessoa, gostos, match e roteiro vindos do app).
   3. Aceitar o lead: ele vira negócio no funil, com valor estimado e uma tarefa.
   4. Criar a proposta a partir do roteiro: destinos, datas e atrações já vêm preenchidos.
   5. Precificar voos, hotéis e serviços: preço por item, total e margem.
   6. Enviar a proposta para o app do grupo.
   7. Simular que o grupo aceitou no app: o negócio vai para "Ganho".
   8. Criar a viagem e cumprir o checklist da sala de embarque.
   9. Lançar despesas do grupo, que aparecem no app como "lançada pela agência".
   10. Simular a viagem quitada: chegam a avaliação e o lead da próxima viagem.
3. Para começar de novo, use **Reiniciar protótipo** no rodapé do menu.

## O que é simulado

- **Todos os nomes, valores, hotéis e companhias aéreas são de exemplo.**
- As ações do lado do grupo (abrir e aceitar a proposta, quitar a viagem) aparecem como botões **Simular**.
- Busca, filtros e "Criar" manual não funcionam neste protótipo.
- Nada é salvo: recarregar a página volta ao início.

## Arquivos

- `index.html`: o protótipo inteiro (HTML, CSS e JavaScript, sem dependências).
- `assets/emo.js`: ícones 3D (Microsoft Fluent Emoji, licença MIT).
- `assets/fotos.js`: fotos do Wikimedia Commons; créditos no repositório do [protótipo do app](https://github.com/flavioantoniojr/apptravel-prototipo/blob/main/creditos-fotos.md).
