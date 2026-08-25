Wiki de Projetos de Curso
Sobre o projeto

A Wiki de Projetos de Curso é um espaço destinado à organização e documentação dos projetos desenvolvidos durante o curso.

1. Índice
Projetos
Contribua

2. Página de Projetos
Projeto	Descrição	Status
Projeto 1	Descrição do primeiro projeto	Em desenvolvimento
Projeto 2	Descrição do segundo projeto	Planejado
Projeto 3	Descrição do terceiro projeto	Planejado

3. Contribua

Para contribuir com o projeto:

Crie uma nova branch a partir da main.
Realize as alterações necessárias.
Faça commits seguindo a convenção definida no projeto.
Envie a branch para o repositório remoto.
Abra um Pull Request para a branch main.
Aguarde a revisão e aprovação das alterações.

-----------------

Como revisar mudanças

Antes de integrar uma branch à main, as alterações devem ser revisadas para garantir que o código esteja organizado e de acordo com as regras do projeto.

Revisão pelo terminal

Para atualizar as informações do repositório remoto:

git fetch origin

Para comparar a branch atual com a main:

git diff origin/main...HEAD

Para visualizar somente os arquivos alterados:

git diff --name-status origin/main...HEAD

Durante a revisão, devem ser verificados:

Arquivos adicionados, modificados ou removidos;
Organização das pastas;
Referências para imagens e outros arquivos;
Alterações no HTML e CSS;
Arquivos que deveriam estar no .gitignore;
Mensagens e granularidade dos commits;
Possíveis problemas antes da integração.
Revisão pelo GitHub

Após publicar a branch no repositório remoto, deve ser aberto um Pull Request para a main.

Na seção Files changed, os integrantes podem visualizar e revisar todas as alterações realizadas antes do merge.

Somente após a revisão e a confirmação de que as alterações estão adequadas, a branch deverá ser integrada à main.