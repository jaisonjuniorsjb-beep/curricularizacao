# Brincando e Aprendendo — Prof. Corujinha

Jogo para Educação Infantil, Pré-escola II (5 a 6 anos), elaborado a partir do protótipo fornecido. Projeto de Curricularização da Extensão: Sistemas de Informação da UNIFEBE em parceria com a Secretaria Municipal de Educação de Brusque. As menções identificam o contexto informado; os conteúdos ainda precisam de validação da equipe pedagógica.

## Executar

Abra `index.html` em Chrome, Firefox ou Edge. Não é necessário instalar dependências, criar contas ou compilar. Os arquivos precisam permanecer na mesma pasta. As perguntas, ilustrações, sons e estilos são locais. A disponibilidade de uma voz em português depende do navegador e do sistema; alguns serviços de voz podem precisar de internet.

## O que está implementado

- Tela inicial, escolha de aventura, dez perguntas por partida, retorno após cada resposta e resultado final.
- Três aventuras, totalizando trinta perguntas: Descobertas; Cores e números; Letras e sons.
- Alternativas embaralhadas a cada partida, com correção e explicação acolhedora.
- Estrelas, resumo das habilidades e reinício da partida.
- Interface adaptável para celular, tablet e computador, controles por teclado, foco visível e botão para ouvir perguntas e alternativas.
- Corujinha em SVG próprio. Sem bibliotecas, imagens externas, fontes remotas, anúncios ou rastreamento.
- Sem cadastro ou armazenamento de resultados. O acompanhamento refere-se à partida atual; os resultados desaparecem ao recarregar a página.

## Publicar no GitHub Pages

Nome solicitado: `curricularização`. Nome técnico previsto: `curricularizacao` (o nome de repositório usa caracteres sem acentos).

1. Criar o repositório público `curricularizacao` na conta responsável.
2. Enviar **o conteúdo desta pasta** para a raiz da branch `main`, incluindo `.github/workflows/pages.yml` e `.nojekyll`.
3. Em **Settings → Pages → Build and deployment → Source**, escolher **GitHub Actions**.
4. Na aba **Actions**, executar ou acompanhar o fluxo **Publicar jogo no GitHub Pages**. Se o envio ocorreu antes de ativar Pages, executar o fluxo manualmente.
5. Quando o fluxo terminar com sucesso, abrir o endereço exibido no ambiente `github-pages` e testar todas as aventuras.

Endereço esperado: `https://SEU-USUARIO.github.io/curricularizacao/`. Esse endereço é um modelo, não um link publicado. A publicação não foi realizada sem conexão e autorização da conta GitHub.

Para publicar pelo envio de arquivos no site do GitHub, confirme que a pasta oculta `.github` também foi incluída. Alternativamente, após enviar os arquivos, é possível escolher **Deploy from a branch**, branch `main`, pasta `/ (root)` em Pages; nesse caso o fluxo de Actions deste pacote não é necessário.

## Validação

Testes automatizados de lógica executados: 9 partidas, 90 respostas, pontuações de 0, 9 e 10 acertos em cada aventura; bloqueio de resposta duplicada; explicações; reinício; escolha de aventura; retorno ao início. Verificação de sintaxe JavaScript aprovada.

Os testes de lógica usam simulação mínima do documento e não substituem testes reais de navegador. A prévia HTTP foi impedida pelas permissões de rede do ambiente de desenvolvimento. A verificação visual e a compatibilidade real em Chrome, Firefox e Edge **ainda precisam ser executadas**. As APIs utilizadas são padrões comuns, mas isso não comprova a compatibilidade.

Consulte `VALIDACAO.md` para o roteiro de testes técnicos, pedagógicos e de experiência do usuário.
