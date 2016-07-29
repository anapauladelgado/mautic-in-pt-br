# mautic-in-pt-br
Translation of the Mautic Documentation form EN to PT-BR
Documentação do Mautic
Introdução
Este livro serve como documentação para o Mautic, o sistema open source de automação de marketing. Assim como o código é aberto e disponível para todos, também o é a sua documentação. Todos são bem-vindos a melhorar estas informações conforme necessário.
Download como PDF
Clique aqui para baixar estes documentos como PDF.
Como contribuir com os documentos
Este repositório é o código fonte de Gitbook publicado em www.mautic.org/docs. O código fonte é compartilhado aqui no GitHub para que qualquer um possa contribuir na documentação da mesma forma que os programadores fazem com o código atual do Mautic.
Por que o git é usado para a documentação
versões. Qualquer pessoa pode voltar atrás e olhar como o texto estava antes.
autoria. Não somente cada arquivo, mas cada linha tem seu próprio autor.
contribuições da comunidade. Não é preciso se preocupar sobre deletar o trabalho de outra pessoa enquanto estiver trabalhando no mesmo documento.
Embora alguns conhecimentos sobre o git sejam necessários para clonar, modificar, “comitar” (commit) e carregar alterações, há uma maneira de evitar isso e editar os arquivos diretamente na interface web do GitHub. Se você conhece git, use o fluxo de trabalho (workflow) que você gosta. Se não, siga este guia que vai lhe mostrar como contribuir com facilidade.
Edite documentos em um navegador
Crie uma nova instância (clique em “Fork”) deste repositório diretamente na sua própria conta para que você tenha permissão para editar.
Selecione um arquivo para editar. A estrutura do arquivo é explicada abaixo. Agora, vamos editar o arquivo README.md para mostrar os princípios. Clique nele.
O conteúdo de README.md deve aparecer, bem como o botão Edit (o ícone de um lápis) acima. Clique nele.
O conteúdo está escrito em Markdown markup. Uma formatação muito simples baseada em texto.
Faça alguma alteração no arquivo. Por exemplo, adicione ao final Esta é a minha primeira contribuição.
Quando você fizer uma alteração, role a tela para baixo e note o formulário chamado “Commit changes”. Isto é importante. Para salvar uma alteração, você tem que descrever o que você mudou e por que. Escreva, por exemplo, Uma nova linha adicionada para fins de teste. Mas, não salve ainda!
Como a interface web GitHub não fornece todos os recursos do git, não teremos uma maneira fácil de reverter a mudança de volta ao estado original. Nós teríamos de criar um outro commit quando deletássemos a linha adicionada. Isso causaria uma bagunça no histórico de commits. Então, em vez disso, cria-se um novo ramo. Há um checkbox para isso "Create a new branch...". O ramo precisa ter um nome. {seuusuário}-patch-1 será previamente preenchido. Vamos alterar isso para {seuusuário}-teste. Agora, clique em Propose file change.
Ok! Agora, a alteração já existe no seu repositório. Para propor a alteração no repositório oficial, você precisa enviar uma solicitação (pull request = PR). Você será redirecionado para fazer exatamente isso. Aqui, você descreve a sua alteração proposta e clica (por favor, não envie as PRs de testes) no botão Create pull request.
Se você quiser limpar após o teste, vá para a seção Branches e exclua o ramo de testes.
A estrutura de arquivo
Estivemos trabalhado com o arquivo README.md na seção anterior. Este arquivo é mostrado na página inicial de um repositório GitHub e você está lendo seu conteúdo no momento. Ele não tem nada a ver com a Documentação Mautic.
O arquivo SUMMARY.md define o menu da documentação. Se você adicionar uma nova página à documentação, você também terá de adicionar uma nova linha lá, definindo o título e o link para o arquivo. É bem simples e direto quando você vir os itens de menu atuais.
As pastas estão aqui para agruparem os tópicos. Abra, por exemplo, a pasta asset. Você verá que ela tem o seu próprio arquivo README.md. É o conteúdo principal quando você clica no item de menu Asset. O arquivo manage_assets.md é um subitem. A subpasta media contem as imagens utilizadas nos arquivos md.
Links
Frequentemente você pode querer criar um link para outro lugar da documentação. Em Markdown, o link se parece com isto:
[título do link](http://exemplo.com)


Isto criará um link externo com URL absoluta. Se você quiser criar um link interno, use a URL relativa como esta:
[estes passos](./../plugins/teste_de_integracao.html)


Isto linkará a plugins/teste_de_integracao.html no site de documentação criado a partir do arquivo fonte md.
Imagens
Como se pode notar acima, as imagens podem ser colocadas nas pastas de mídia (media). Provavelmente não será possível subir imagens através da interface web do GitHub, mas você pode subi-las para qualquer URL pública e linká-las a partir daí.
![texto alternativo aqui](http://exemplo.com/images/apple.png "Texto de dica aqui")


Ou, se você quiser exibir uma imagem já existente no repositório da documentação, você poderá usar um caminho relativo:
![texto alternativo aqui](/assets/media/assets-novacategoria.png "Texto de dica aqui")


*Nota de tradução: optamos por manter os termos referentes à plataforma utilizada no original em inglês, uma vez que ela está nesse idioma, e também porque é muito comum usarmos certos estrangeirismos no jargão técnico, como em “comitar”, por exemplo.
