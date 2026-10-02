Análise de Requisitos — Plataforma de Estudos Gamificada
1 de out. de 2026 · @Gabriel
1. Visão geral
Plataforma de estudos web e mobile, de uso pessoal. O usuário organiza o estudo em matérias e submatérias, e cada lista de exercícios vira uma trilha: a cada acerto, o Pokémon escolhido ataca um Pokémon selvagem, e uma nota de 70% ou mais o captura. Não é um jogo: batalha, evolução e captura são a recompensa pelo estudo.
Objetivo. Tornar o estudo de qualquer assunto uma sequência guiada: resumo da submatéria, questões no nível escolhido, explicação após cada resposta e progresso visível do Pokémon.
Público. Uso pessoal do autor, estudante de Ciência da Computação. O código fica em repositório público, sem as imagens de Pokémon; o sistema não será publicado nem usado comercialmente.
Diferencial. Não existe catálogo de conteúdo. O usuário descreve cada submatéria em um prompt, e a IA gera o resumo e as questões abertas e fechadas, em três níveis, com gráficos, diagramas e fórmulas quando o assunto pede. Provas e listas enviadas servem de modelo de estilo.
2. Escopo
O MVP entrega o ciclo completo: tutorial, matérias e submatérias, listas com batalha e captura, coleção e evolução. App mobile nativo e recursos de engajamento ficam para a versão seguinte.
Funcionalidade
Entrega
Cadastro e login
MVP
Tutorial com escolha do inicial (Bulbasaur, Charmander ou Squirtle)
MVP
Matérias (só nome) e submatérias (descrição, prompt e materiais)
MVP
Resumo da submatéria gerado pela IA
MVP
Listas como trilhas, com batalha e captura com nota de 70% ou mais
MVP
Questões abertas (corrigidas pela IA) e fechadas (vários formatos)
MVP
Listas fáceis, médias, difíceis ou com todas as dificuldades
MVP
Explicação após cada resposta
MVP
Gráficos, diagramas, desenhos e fórmulas gerados pela IA
MVP
Raridade dos Pokémon selvagens conforme a dificuldade
MVP
Coleção com pesquisa e filtro, card do Pokémon, evolução e mega evolução
MVP
Upload de provas e listas (PDF e imagem) como referência
MVP
Download da lista em PDF
MVP
Versão web instalável (PWA)
MVP
App mobile nativo (Expo)
Versão seguinte
Revisão espaçada das questões erradas
Versão seguinte
Ofensiva de dias e notificações
Versão seguinte
Fora do escopo. Questões avulsas fora de listas, batalhas entre usuários, publicação das imagens de Pokémon e uso comercial.
3. Glossário
Termo
Significado
Matéria
Agrupador de estudo identificado só pelo nome (ex.: Teoria dos Grafos).
Submatéria
Assunto dentro de uma matéria (ex.: Dijkstra, DFS, BFS), com descrição, prompt e materiais; é a base para a IA gerar conteúdo.
Prompt da submatéria
Texto em que o usuário explica à IA o que quer estudar.
Resumo
Explicação geral da submatéria gerada pela IA.
Material de referência
Prova ou lista (PDF ou imagem) enviada para a IA imitar o estilo das questões.
Lista (trilha)
Lista de exercícios de uma ou mais submatérias, exibida como um caminho com paradas.
Parada
Ponto da trilha; contém exatamente uma questão.
Questão aberta
Resposta em texto livre, corrigida pela IA como certa (100%), aceitável (50%) ou errada (0%).
Questão fechada
Resposta exata, vale 100% ou 0%: resposta única, múltipla escolha (uma ou mais corretas), verdadeiro/falso, lacuna, associar colunas, ordenar ou numérica.
Resposta modelo
Resposta ideal de uma questão aberta, usada na correção e mostrada ao usuário depois.
Recurso visual
Gráfico, diagrama, desenho, fórmula, tabela ou código gerado pela IA.
Dificuldade
Fácil, médio, difícil ou todas (mistura dos três na mesma lista).
Nota da lista
Média das pontuações das paradas, de 0 a 100%.
Espécie
Pokémon do catálogo, com sprite, linha evolutiva, raridade e, se existir, forma mega.
Raridade
Classificação da espécie (comum, incomum ou rara) que define em qual dificuldade ela aparece como selvagem.
Pokémon inicial
Bulbasaur, Charmander ou Squirtle, escolhido no tutorial.
Coleção
Todos os Pokémon do usuário: o inicial e os capturados.
Pokémon da lista
Pokémon da coleção escolhido para seguir uma lista; recebe o XP dela.
Pokémon selvagem
Pokémon sorteado para a lista, atacado a cada acerto.
Captura
Entrada do selvagem na coleção quando a nota da lista é de 70% ou mais.
Evolução
Passagem para a próxima espécie da linha evolutiva ao atingir o nível exigido.
Mega evolução
Forma final em nível muito alto (ex.: 100), só para espécies que têm forma mega.
4. Atores
• Estudante (usuário): cria matérias e submatérias, envia provas e listas, cria e resolve listas, captura Pokémon e acompanha o progresso.
• Serviço de IA (externo): analisa o material de referência, gera resumos, questões e recursos visuais, e corrige as respostas abertas.
5. Telas
Baseadas nos rascunhos do autor. Toda resolução de lista segue o layout desenhado no tutorial.
Tela
Conteúdo
T01 Login
Nome do site, e-mail, senha e link "cadastre-se".
T02 Cadastro
Nome completo, e-mail, senha, confirmação de senha e nível de ensino.
T03 Tutorial
Escolha do inicial; lista de exemplo com uma questão (ex.: capital da França); ✓ e ✗ no caminho; demonstração dos três finais: captura (70% ou mais), fuga (50% a menos de 70%) e desmaio (abaixo de 50%).
T04 Início
Estatísticas gerais (questões feitas, listas feitas, média de acertos) e botões Minhas listas, Meus Pokémon e Criar matéria.
T05 Listas
Matérias na lateral com "+ nova matéria"; listas a fazer (com o selvagem de cada uma), em andamento e já feitas (nota e refazer); botão "+ criar lista".
T06 Nova matéria
Apenas o nome.
T07 Criar submatéria
Nome, descrição, upload de provas e listas (PDF ou imagem) e prompt para a IA; ao salvar, a IA gera o resumo.
T08 Resumo da submatéria
Resumo com recursos visuais e acesso às listas da submatéria.
T09 Nova lista
Nome, quantidade de questões, submatérias (uma ou mais), dificuldade (fácil, médio, difícil ou todas) e tipo (fechada, aberta ou todos).
T10 Escolher Pokémon
Ao abrir uma lista, grade da coleção com pesquisa para escolher quem segue a trilha.
T11 Resolver lista
Caminho com paradas, Pokémon do usuário, selvagem com barra de vida e questão com a área de resposta do formato. Após responder: resultado, explicação, resposta modelo (abertas), contestar e reportar. Também: reabrir resumo, sair e baixar PDF.
T12 Resultado da lista
Nota, XP, evolução ou mega, animação de captura, fuga ou desmaio, e botão refazer.
T13 Meus Pokémon
Coleção com pesquisa e filtro.
T14 Card do Pokémon
Nível, barra de XP até o próximo nível, questões e listas feitas com ele, e apelido.
T15 Perfil
Nível de ensino e sair da conta.
6. Requisitos funcionais
São 66 requisitos em 10 módulos. Prioridade Alta = obrigatório no MVP; Média = desejável no MVP; Baixa = versão seguinte.
6.1 Conta e tutorial
ID
Requisito
Prioridade
RF01
O usuário deve se cadastrar com nome completo, e-mail, senha e confirmação de senha.
Alta
RF02
O usuário deve fazer login e permanecer autenticado por token.
Alta
RF03
O usuário deve definir seu nível de ensino (médio, graduação, pós), usado pela IA para calibrar o conteúdo.
Média
RF04
O usuário deve poder recuperar a senha por e-mail.
Baixa
RF05
No primeiro acesso, um tutorial deve permitir escolher o Pokémon inicial: Bulbasaur, Charmander ou Squirtle.
Alta
RF06
O tutorial deve demonstrar uma lista curta com questão de exemplo, ✓ e ✗ no caminho e os três finais possíveis: captura, fuga e desmaio.
Alta
RF07
O usuário deve poder pular o restante do tutorial depois de escolher o inicial.
Média
6.2 Matérias e submatérias
ID
Requisito
Prioridade
RF08
O usuário deve criar uma matéria informando apenas o nome.
Alta
RF09
As matérias devem aparecer na lateral da tela de listas, com o botão "+ nova matéria".
Alta
RF10
O usuário deve criar submatérias dentro de uma matéria, com nome, descrição, prompt para a IA e materiais opcionais.
Alta
RF11
A IA deve confirmar que o prompt descreve um assunto real e recusar o que não for.
Alta
RF12
Ao criar a submatéria, a IA deve gerar um resumo geral do assunto.
Alta
RF13
O resumo deve ser salvo; o usuário pode pedir para regerar.
Alta
RF14
O resumo deve aceitar formatação rica e recursos visuais.
Média
RF15
O usuário deve poder renomear, arquivar e excluir matérias e submatérias.
Média
6.3 Material de referência
ID
Requisito
Prioridade
RF16
O usuário deve enviar provas e listas em PDF ou imagem ao criar ou editar uma submatéria.
Alta
RF17
O usuário deve marcar cada arquivo como prova ou lista.
Média
RF18
A IA deve analisar cada arquivo uma única vez e salvar um perfil de estilo: formatos, profundidade e nível.
Alta
RF19
Ao gerar questões, a IA deve seguir o perfil de estilo da submatéria, sem copiar questões do material.
Alta
RF20
O usuário deve poder listar, visualizar e excluir os materiais enviados.
Média
6.4 Listas
ID
Requisito
Prioridade
RF21
O usuário deve criar uma lista com nome, quantidade de questões, uma ou mais submatérias, dificuldade (fácil, médio, difícil ou todas) e tipo (fechada, aberta ou todos).
Alta
RF22
A tela de listas deve separar listas a fazer, em andamento e já feitas, mostrando o selvagem e a melhor nota de cada uma.
Alta
RF23
Ao abrir uma lista, o usuário deve escolher qual Pokémon da coleção a segue, com pesquisa.
Alta
RF24
A lista deve ser exibida como caminho com paradas, no mesmo layout do tutorial.
Alta
RF25
As paradas devem ser liberadas em sequência; a seguinte só abre após responder a atual.
Alta
RF26
Cada parada deve conter exatamente uma questão.
Alta
RF27
Após responder, o Pokémon do usuário deve andar até a próxima parada.
Alta
RF28
O usuário deve poder reabrir o resumo da submatéria durante a lista.
Alta
RF29
O usuário deve poder sair e continuar a lista de onde parou.
Alta
RF30
O usuário deve poder refazer uma lista já feita.
Alta
RF31
O usuário deve poder baixar uma lista em PDF para estudar sem internet.
Média
6.5 Batalha e captura
ID
Requisito
Prioridade
RF32
Cada lista deve ter um Pokémon selvagem sorteado conforme a raridade ligada à dificuldade, com barra de vida visível.
Alta
RF33
A cada resposta pontuada, o Pokémon do usuário deve atacar o selvagem com dano proporcional à pontuação; o erro só marca ✗ no caminho.
Alta
RF34
Ao terminar, o sistema deve mostrar nota, acertos, erros, XP ganho e evolução, se houve.
Alta
RF35
Com nota de 70% ou mais, deve aparecer o Pokémon do usuário derrotando o selvagem e a captura; o Pokémon vai para a coleção.
Alta
RF36
Com nota de 50% a menos de 70%, deve aparecer o selvagem fugindo.
Alta
RF37
Com nota abaixo de 50%, deve aparecer o selvagem atacando e o Pokémon do usuário desmaiando.
Alta
6.6 Questões e correção
ID
Requisito
Prioridade
RF38
O sistema deve ter dois tipos de questão: abertas e fechadas.
Alta
RF39
As fechadas devem suportar resposta única, múltipla escolha (uma ou mais corretas), verdadeiro/falso, lacuna, associar colunas, ordenar e numérica, cada uma com sua área de resposta.
Alta
RF40
Cada questão deve ter dificuldade: fácil, médio ou difícil.
Alta
RF41
Após responder, o sistema deve mostrar o resultado, a resposta correta e a explicação.
Alta
RF42
Nas abertas, o usuário responde em texto livre e a IA corrige como certa (100%), aceitável (50%) ou errada (0%), com justificativa.
Alta
RF43
Após a correção de uma aberta, o sistema deve mostrar a resposta modelo.
Alta
RF44
O usuário deve poder contestar a correção de abertas quantas vezes quiser; fechadas não têm contestação.
Baixa
RF45
O usuário deve poder reportar uma questão como errada ou confusa.
Média
6.7 Pokémon e coleção
ID
Requisito
Prioridade
RF46
O sistema deve ter um catálogo de espécies com sprite, tipo, linha evolutiva, nível de evolução, raridade e forma mega, quando existir.
Alta
RF47
A tela Meus Pokémon deve listar a coleção com pesquisa e filtro.
Alta
RF48
O card do Pokémon deve mostrar nível, barra de XP até o próximo nível e quantas questões e listas foram feitas com ele.
Alta
RF49
O Pokémon que segue a lista deve ganhar XP a cada acerto e subir de nível.
Alta
RF50
O Pokémon deve evoluir ao atingir o nível de evolução da espécie, com animação.
Alta
RF51
Em nível muito alto, o Pokémon deve mega evoluir, se a espécie tiver forma mega.
Alta
RF52
O usuário deve poder dar apelido a um Pokémon.
Baixa
6.8 Recursos visuais
ID
Requisito
Prioridade
RF53
A IA deve incluir recursos visuais quando o assunto pedir: gráficos, diagramas, grafos, desenhos geométricos, fórmulas, tabelas e código.
Alta
RF54
Os visuais podem aparecer no enunciado, nas alternativas, na explicação e no resumo.
Alta
RF55
A IA deve gerar os visuais como dados (especificação de gráfico, Mermaid, LaTeX ou SVG), e o front deve desenhá-los.
Alta
RF56
Ao corrigir uma aberta, a IA deve receber também o visual da questão.
Média
6.9 Progresso
ID
Requisito
Prioridade
RF57
A tela inicial deve mostrar questões feitas, listas feitas e média de acertos.
Alta
RF58
O sistema deve registrar cada resposta: questão, resposta dada, pontuação e tempo.
Alta
RF59
Cada matéria e submatéria deve mostrar acerto por nível, listas feitas e Pokémon capturados.
Média
RF60
O sistema deve permitir revisar as questões erradas.
Baixa
6.10 Integração com IA
ID
Requisito
Prioridade
RF61
A IA deve gerar conteúdo para qualquer assunto, sem cadastro prévio de temas.
Alta
RF62
A IA deve respeitar o nível: fácil = definições e reconhecimento direto; médio = aplicar um conceito; difícil = combinar conceitos, cálculos em várias etapas ou casos de borda.
Alta
RF63
O back deve ser o único a chamar a IA; o front nunca acessa a API diretamente.
Alta
RF64
A IA deve devolver JSON em formato fixo; o back valida e, se inválido, tenta de novo até 3 vezes.
Alta
RF65
Todo conteúdo gerado deve estar em português do Brasil.
Alta
RF66
O sistema deve mostrar um estado de carregamento enquanto a IA gera ou corrige.
Alta
7. Regras de negócio
São 24 regras em três grupos: conteúdo, pontuação e batalha, e Pokémon e XP.
7.1 Conteúdo e questões
ID
Regra
RN01
Toda questão pertence a uma parada de uma lista; não existem questões fora de listas.
RN02
Toda questão tem explicação; sem ela, não é salva.
RN03
Questões de alternativas têm de 3 a 5 opções: resposta única tem exatamente uma correta; múltipla escolha tem uma ou mais.
RN04
Toda aberta é gerada com resposta modelo e critérios de correção; sem eles, não é salva.
RN05
O tipo da lista (fechada, aberta ou todos) é escolhido na criação e não muda depois.
RN06
Com dificuldade fácil, médio ou difícil, todas as questões têm esse nível; com "todas", a lista mistura os três.
RN07
A lista é gerada inteira antes de começar; as questões não mudam durante a tentativa.
RN08
Uma lista pode abranger uma ou mais submatérias da mesma matéria.
RN09
Uma submatéria só é criada se a IA confirmar que o prompt descreve um assunto real.
RN10
A IA usa o material de referência como modelo de estilo e nunca repete questões dele literalmente.
RN11
Todo recurso visual passa por validação de formato; se falhar, a questão é gerada de novo.
7.2 Pontuação e batalha
ID
Regra
RN12
Fechadas valem 100% ou 0%; a múltipla escolha só vale 100% se marcar todas as corretas e nenhuma errada. Abertas valem 100% (certa), 50% (aceitável) ou 0% (errada).
RN13
Nota da lista = média das pontuações das paradas.
RN14
Errar não causa dano a nenhum Pokémon, inclusive no tutorial. O dano de cada questão é proporcional à pontuação, e a vida do selvagem vale 70% do dano máximo da lista.
RN15
Resultado pela nota: abaixo de 50%, o Pokémon do usuário desmaia; de 50% a menos de 70%, o selvagem foge; 70% ou mais, o selvagem é derrotado e capturado.
RN16
Uma resposta enviada não pode ser alterada.
RN17
A correção de abertas pode ser contestada sem limite; fechadas não têm contestação.
Cálculo da vida do selvagem (RN14). Com N paradas e D de dano por acerto completo:
\text{dano}_i = \frac{\text{pontuação}_i}{100} \cdot D \qquad \text{vida} = 0{,}7 \cdot N \cdot D
O selvagem cai exatamente quando a nota chega a 70%. Exemplo: com 10 paradas e D = 10, a vida é 70; 7 acertos derrotam, enquanto 6 acertos e uma aberta aceitável (65) não.
7.3 Pokémon e XP
ID
Regra
RN18
O primeiro Pokémon é o inicial escolhido no tutorial; os demais vêm apenas de capturas em listas.
RN19
Só Pokémon da coleção podem seguir uma lista; o escolhido recebe o XP dela, e o XP fica com ele.
RN20
O XP de uma questão só é ganho na primeira vez que ela é acertada, e cada lista só captura uma vez. Refazer não dá XP nem nova captura.
RN21
O selvagem é sorteado aleatoriamente entre as espécies da raridade ligada à dificuldade: fácil → comuns, médio → incomuns, difícil → raras.
RN22
A mega evolução só ocorre em espécies com forma mega, em nível muito alto (ex.: 100); as demais não mudam nesse nível.
RN23
Uma espécie tem forma mega se existir arquivo de mega para ela (ID-Mega.png, ID-Mega-X.png ou ID-Mega-Y.png).
RN24
Um Pokémon nunca regride: não desfaz evolução nem mega evolução.
8. Requisitos não funcionais
ID
Categoria
Requisito
RNF01
Tecnologia
O back-end deve ser escrito em C++ e expor uma API REST com JSON.
RNF02
Tecnologia
O banco de dados deve ser PostgreSQL.
RNF03
Plataforma
O front web deve funcionar em navegadores modernos e ser instalável como PWA; o mobile virá depois com React Native (Expo).
RNF04
Segurança
Senhas com hash Argon2, autenticação por JWT e tráfego somente via HTTPS.
RNF05
Segurança
A chave da API de IA fica apenas no servidor, em arquivo .env fora do Git.
RNF06
Segurança
SVG e HTML gerados pela IA são sanitizados antes de exibir, sem scripts.
RNF07
Desempenho
Endpoints sem IA respondem em menos de 300 ms.
RNF08
Desempenho
Uma lista de 10 questões é gerada em até 30 s, com progresso visível.
RNF09
Desempenho
A correção de uma resposta aberta leva até 10 s, com indicador de carregamento.
RNF10
Arquivos
Uploads aceitam PDF, JPG e PNG de até 20 MB, guardados em volume do servidor.
RNF11
Dados
A base de espécies vem do dataset JSON do repositório HybridShivam/Pokemon, importada por script; as imagens comprimidas usadas ficam em assets/pokemon/ e nada é carregado do GitHub em tempo de uso.
RNF12
Custo
Limite diário de gerações (ex.: 10 listas) e análise de cada upload uma única vez.
RNF13
Usabilidade
Interface mobile-first, utilizável com uma mão, em telas a partir de 360 px.
RNF14
Usabilidade
Animações de ataque, evolução, captura, fuga e desmaio são feitas com CSS / Framer Motion sobre as artes estáticas, duram até 3 s e podem ser puladas.
RNF15
Idioma
Interface e conteúdo em português do Brasil.
RNF16
Manutenibilidade
Testes automáticos nas regras de nota, dano, captura, sorteio por raridade, XP e evolução.
RNF17
Implantação
Back e banco empacotados com Docker Compose; rodam no PC do autor e podem migrar para uma VPS sem mudança de código.
RNF18
Repositório
O código fica em repositório público; assets/pokemon/ e .env ficam no .gitignore, e um script baixa as imagens localmente.
9. Arquitetura e decisões técnicas
O back em C++ é o centro do sistema: os clientes só falam com ele, e só ele acessa o banco e a IA.
Camada
Escolha
Motivo
Framework HTTP
Drogon (C++17)
Rotas REST, JSON, ORM para PostgreSQL, upload de arquivos e cliente HTTP no mesmo pacote.
Banco
PostgreSQL, com libpqxx ou o ORM do Drogon
Relacional para quase tudo; JSONB para recursos visuais e perfil de estilo.
JSON
jsoncpp (incluso no Drogon) ou nlohmann/json
Ler e validar o retorno da IA.
Autenticação
jwt-cpp + libsodium (Argon2)
Token e hash de senha.
IA
Chamada REST direta à API, sem SDK
Não há SDK oficial em C++; o prompt exige JSON em formato fixo.
Provas e listas
Arquivo enviado à IA como documento ou imagem
A API lê PDF e imagem, inclusive digitalizados, sem OCR próprio; a análise vira um perfil de estilo salvo.
Recursos visuais
Front desenha: Recharts (gráficos), Mermaid (diagramas), KaTeX (fórmulas), Cytoscape.js (grafos), SVG sanitizado com DOMPurify
A IA gera só dados; desenhar no front é mais confiável que pedir imagens prontas.
PDF da trilha
Gerado no front
Evita biblioteca de PDF em C++ e reaproveita os componentes de exibição.
Pokémon
Artes e dataset do repositório HybridShivam/Pokemon, copiados para assets/pokemon/ e importados por script
Sem dependência externa em tempo de uso.
Build e implantação
CMake + vcpkg ou Conan; Docker Compose
Gerenciar dependências C++ e subir back e banco com um comando.
Front web
React + TypeScript, PWA
Instalável no celular desde o MVP.
Mobile
React Native com Expo, em monorepo com o web
Reaproveita tipos e regras em TypeScript.
Animações
CSS / Framer Motion sobre as artes estáticas
O repositório não tem sprite sheets; pulo, tremor, piscar e encolher bastam para ataque, dano, evolução e desmaio.
Todo conteúdo gerado pela IA é salvo no banco: a IA só é chamada para criar algo novo ou corrigir uma resposta aberta, nunca para exibir algo existente.
10. Modelo de dados
São 13 tabelas. A espécie é o catálogo; cada registro em pokemon é um exemplar da coleção do usuário. As estatísticas do card e da tela inicial são calculadas a partir de tentativa e resposta.
Tabela
Campos principais
Observação
usuario
id, nome, email, senha_hash, nivel_ensino, tutorial_concluido, criado_em

especie
id, numero_pokedex, nome, tipos, sprite, evolui_para_id, nivel_evolucao, raridade (comum, incomum, rara), sprites_mega, nivel_mega
Catálogo; campos mega nulos sem forma mega.
pokemon
id, usuario_id, especie_id, apelido, nivel, xp, mega_evoluido, origem (inicial ou captura), obtido_em
Coleção do usuário.
materia
id, usuario_id, nome, arquivada, criada_em
Só o nome.
submateria
id, materia_id, nome, descricao, prompt, resumo, criada_em
Base para a IA.
material_referencia
id, submateria_id, tipo (prova ou lista), caminho_arquivo, perfil_estilo (JSONB), enviado_em
Perfil gerado uma vez pela IA.
lista
id, materia_id, nome, quantidade, dificuldade (facil, medio, dificil, todas), tipo (fechada, aberta, todos), especie_selvagem_id, vida_selvagem, capturada, criada_em
capturada impede segunda captura.
lista_submateria
lista_id, submateria_id
Uma lista cobre uma ou mais submatérias.
parada
id, lista_id, ordem, questao_id
Posição no caminho.
questao
id, submateria_id, tipo (aberta ou fechada), formato, dificuldade, enunciado, visual (JSONB), resposta_modelo, criterios_correcao, explicacao, ja_acertada, reportada
Formato: resposta única, múltipla escolha, V/F, lacuna, associar, ordenar, numérica ou texto.
alternativa
id, questao_id, texto, correta, ordem
Mais de uma correta na múltipla escolha.
tentativa
id, lista_id, pokemon_usado_id, parada_atual, status, nota, resultado (desmaio, fuga ou captura), iniciada_em, concluida_em
Permite continuar e refazer.
resposta
id, tentativa_id, parada_id, alternativas_marcadas ou texto_resposta, pontuacao (0, 50 ou 100), feedback_ia, contestacoes, tempo_ms, xp_ganho
Base de nota, dano, XP e estatísticas.
Relacionamentos: usuario 1–N pokemon e materia; especie 1–N pokemon; materia 1–N submateria e lista; submateria 1–N material_referencia e questao; lista N–N submateria (via lista_submateria); lista 1–N parada e tentativa; parada N–1 questao; questao 1–N alternativa; tentativa 1–N resposta. Ao capturar, um novo registro em pokemon é criado.
11. Fluxo principal do usuário
O usuário cria a matéria e a submatéria uma vez e depois repete o ciclo lista → paradas → resultado quantas vezes quiser.
Errar não causa dano: no caminho "não" de Acertou?, o Pokémon apenas não ataca. "Foge ou desmaia" corresponde à nota de 50% a menos de 70% (fuga) ou abaixo de 50% (desmaio); depois disso, o usuário pode refazer a trilha, sem XP repetido.
12. Riscos
Risco
Impacto
Mitigação
Imagens de Pokémon são propriedade da Nintendo / The Pokémon Company, e o repositório será público
Remoção do repositório
Imagens fora do Git, baixadas por script (RNF18); o repositório de imagens usado declara o mesmo copyright.
IA gerar gabarito ou explicação errados
Usuário aprende errado
Reportar questão (RF45) e revisão da própria saída pela IA antes de salvar.
IA corrigir uma aberta de forma injusta
Nota e captura injustas
Resposta modelo e critérios fixos (RN04) e contestação ilimitada (RN17).
IA errar o nível de dificuldade
Listas desbalanceadas
Critérios de cada nível no prompt (RF62) e perfil de estilo das provas reais.
Raridades mal distribuídas
Coleção cresce rápido ou devagar demais
Raridade como campo da espécie, ajustável sem mudar código.
Recurso visual mal gerado
Questão ilegível
Validação de formato e nova geração (RN11).
Ecossistema web pequeno em C++
Desenvolvimento mais lento
Drogon e libpqxx; escopo do MVP enxuto.
Sem SDK oficial da API de IA para C++
Mais código manual
Chamada REST direta com o cliente HTTP do Drogon ou libcurl.
Custo de PDFs grandes e correções de abertas
Gasto maior com IA
Análise única de cada upload e limite diário (RNF12).
Latência da IA (10 a 30 s)
Espera longa
Gerar a lista em segundo plano, mostrando o selvagem enquanto carrega.
13. Decisões e pendências
As decisões abaixo já estão refletidas nos requisitos indicados. A lista seguinte reúne o que ainda falta definir.
Tema
Decisão
Referência
Estrutura do estudo
Matéria (só nome) → submatérias (descrição, prompt e materiais) → listas de uma ou mais submatérias.
RF08–RF12, RN08
Questões avulsas
Retiradas; existem apenas listas.
RN01
Tipos de questão
Aberta (corrigida pela IA, 100/50/0%) e fechada (todos os formatos, 100/0%).
RF38, RF39, RN12
Múltipla escolha
Uma ou mais corretas; só vale 100% acertando todas e nenhuma errada.
RN03, RN12
Dificuldade
Fácil, médio, difícil ou todas (mistura).
RN06
Primeiro Pokémon
Inicial escolhido no tutorial.
RF05, RN18
Pokémon da lista
Escolhido ao abrir cada lista; recebe o XP.
RF23, RN19
Pokémon selvagem
Sorteado aleatoriamente, com raridade conforme a dificuldade.
RF32, RN21
Resultado da lista
Abaixo de 50%, desmaio; de 50% a menos de 70%, fuga; 70% ou mais, captura.
RN15, RF35–RF37
Erro
Não causa dano, inclusive no tutorial; só marca ✗.
RN14, RF33
Tela de resolução
Todas as listas seguem o layout do tutorial.
RF24, T11
XP e captura
XP uma única vez por questão; captura uma única vez por lista.
RN20
Mega evolução
Nível muito alto (ex.: 100); detectada pelo nome do arquivo.
RN22, RN23
Contestação
Ilimitada em abertas; inexistente em fechadas.
RN17, RF44
Upload
Provas e listas em PDF ou imagem, na submatéria.
RF16
Uso offline
Download da lista em PDF.
RF31
Imagens
Repositório HybridShivam/Pokemon, fora do Git público.
RNF11, RNF18
Hospedagem
Docker Compose; no PC do autor primeiro, VPS depois se necessário.
RNF17
Valores de XP
Definidos em etapa posterior.
—
[ ] Critério de raridade: como classificar cada espécie em comum, incomum ou rara (ex.: estágio evolutivo, lendários como raros)?
[ ] Dificuldade "todas": de qual raridade vem o selvagem?
[ ] Megas duplas: Charizard e Mewtwo têm Mega X e Mega Y. Usar uma fixa, sortear ou deixar o usuário escolher?
[ ] Nome do site: aparece no login e no cadastro.
[ ] Valores de XP: XP por acerto, por dificuldade e por nível do Pokémon.
Fontes
• HybridShivam/Pokemon: artes oficiais comprimidas e em alta qualidade, formas mega e dataset de espécies da PokéAPI em JSON e CSV.