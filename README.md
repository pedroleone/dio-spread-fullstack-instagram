# Clone da Página de Login do Instagram

Projeto criado para entregar como desafio do Módulo II do Bootcamp Spread Fullstack Developer.

**Objetivo**: Recriar a página de login do Instagram utilizando os conhecimentos HTML e CSS aprendidos.

## Execução do projeto

A página de Login do Instagram foi clonada com base na página de login obtida no dia 05/05/2022 da página principal do [Instagram](https://instagram.com). A diferença em relação ao projeto proposto é que eu **decidi fazer a página de login sem as informações da conta salva**, mostrando ao invés disso os inputs de login e senha. Isso deixou a implementação mais complexa, pois tive que estilizar o formulário e mais informações do que a página modelo proposta pela instrutora.

## Aprendizado

O desafio me ajudou nos seguintes pontos:

* Não digitei nenhuma linha de CSS sem saber exatamente o que ela significava. Por mais que existam soluções prontas na internet para muitos desafios que enfrentei no projeto, copiar e colar não serve como aprendizado.
* Reforçou a idéia de flex-container e flex-item, e que um flex-item pode ser por si só um flex-container também. Utilizei muito esta técnica para subdividir o layout e deixar da forma que esperava.
* Utilizei a ferramenta [ruler](https://github.com/andrijac/ruler) para obter as medidas exatadas do layout original, e a extensão [ColorZilla](https://addons.mozilla.org/pt-BR/firefox/addon/colorzilla/) para obter o código das cores utilizadas.
* Utilizei também o Dev Tools do Firefox para inspecionar elementos e compreender o layout original, mas sem copiar o CSS original.
* O placeholder dos inputs não está exatamente igual ao original. Pesquisei como fazer, e é colocado um span ocupando o mesmo espaço do input, e quando o input recebe o foco um evento no javascript é disparado que diminui o texto e permite escrever enquanto vê o placeholder. Como preferia que este desafio ficasse apenas no HTML e CSS, resolvi não implementar esta funcionalidade.
* O carrossel de imagens foi desafiador, pois nunca tinha desenvolvido animações em CSS. Minha primeira tentativa foi deixar um div com tamanho fixo e alterar a imagem de fundo (background-image) e a opacidade do div nos keyframes. O problema desta solução é que background-image não é animável, enquanto opacidade sim. Então parti para outra solução: as imagens são colocadas sobrepostas no HTML, com position: absolute, uma em cima da outra. Depois, uma única animação foi criada para mexer com a opacidade, alternando entre 0 e 1, e em seguida cada imagem recebe a animação com um delay diferente. 

