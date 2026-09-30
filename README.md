# Ajude a Raposa 🦊🍇

Jogo de Língua Portuguesa para o 6º ano, com reconto didático de A Raposa e as Uvas, interpretação de texto e pronomes.

## Executar

Abra `index.html` no navegador. O arquivo fica na raiz e reúne HTML, CSS e JavaScript, sem dependências externas.

## Fluxo e autenticação

Não há autenticação de alunos, servidor de aplicação, credenciais, tokens, cookies de aplicação ou armazenamento local. O navegador solicita `index.html` ao GitHub Pages por HTTPS; o HTML apresenta as telas, o CSS cuida do visual responsivo e o JavaScript executa o jogo no navegador.

`startGame()` zera `i` e `points`. `render()` apresenta uma das cinco perguntas e três alternativas. `answer()` bloqueia respostas repetidas com `locked`, desabilita os botões, informa a resposta e soma 10 pontos por acerto. `nextQuestion()` só avança depois da resposta. `finish()` apresenta o resultado de 0 a 50. Jogar novamente reinicia a atividade. Recarregar a página perde o progresso, pois ele existe apenas em memória.

A autenticação do proprietário para editar o repositório é separada do jogo: é gerenciada pelo GitHub e pela conexão usada para editar. Nenhuma credencial dessa conexão deve ser colocada no HTML.

## Publicar

No repositório, abra Settings → Pages. Em Build and deployment, selecione Source: Deploy from a branch, branch: main, pasta: / (root), e Save. Aguarde a conclusão da publicação.

Endereço esperado: https://deboraassis-cyber.github.io/Ajude-a-raposa-/

## Validação

A lógica foi testada para cinco perguntas com três alternativas, resultado de 50 e de 0 pontos, respostas mistas, bloqueio de pontuação duplicada, avanço sem resposta e reinício. A publicação deve ser verificada separadamente no endereço público.
