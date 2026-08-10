Semana da Cultura Japonesa

Este projeto é um site simples feito em HTML e CSS para divulgar um evento fictício chamado Semana da Cultura Japonesa.

O evento acontece nos dias 18, 19 e 20 de setembro de 2026, no Centro Cultural do Bairro das Flores, em São Paulo - SP. A ideia foi montar um site com informações sobre as atividades, horários, comidas, imagens e formas de contato.

Organização do site

Eu preferi separar o conteúdo em várias páginas para não deixar tudo dentro do index.html.

Os arquivos ficaram assim:

index.html - página inicial e apresentação do evento;
programacao.html - mostra as oficinas, degustações, palestras e apresentações culturais;
cronograma.html - mostra os dias e horários das atividades;
cardapio.html - mostra alguns pratos, bebidas e acompanhamentos;
galeria.html - mostra imagens relacionadas ao evento;
video.html - página com o vídeo de divulgação;
contato.html - informações de ingresso, contato e formulário de inscrição.

Todas as páginas usam o mesmo menu de navegação, então dá para passar de uma página para outra pelos links no topo.

Escolhas feitas para o evento

O evento foi pensado para durar três dias e misturar culinária e cultura japonesa.

Na programação coloquei oficina de sushi e ramen, degustação de chás e doces, palestras e apresentações culturais. No cronograma também coloquei horários e responsáveis fictícios para cada atividade.

No cardápio aparecem sushi, ramen e chá verde, além de alguns acompanhamentos como gyoza, missoshiru e mochi.

Também coloquei uma galeria com imagens de ambientação, ingredientes e oficina, uma página com vídeo e uma página de contato com um formulário simples.

Onde usei os requisitos da atividade
4.1 HTML

Estrutura básica do HTML5

Todas as páginas possuem DOCTYPE html, html, head e body.

Também usei:

lang=pt-BR;
meta charset=UTF-8;
meta name=viewport;
título da página com title;
meta description;
ligação com o arquivo externo css/estilo.css.

Essas partes ficam no começo de todos os arquivos HTML.

Navegação

O menu foi feito com a tag nav e com links usando a.

Exemplo: no index.html, o menu possui links para programacao.html, cronograma.html, cardapio.html, galeria.html, video.html e contato.html.

Títulos

Usei h1, h2 e h3 para separar os títulos do site e dos conteúdos.

O h1 aparece no cabeçalho com o nome do evento. Os h2 são usados nos títulos principais das páginas e os h3 nos blocos menores, como pratos e atividades.

Imagens

As imagens aparecem em várias páginas, por exemplo:

index.html - imagem de capa;
programacao.html - imagem da oficina;
cardapio.html - imagens de sushi, ramen e chá;
galeria.html - imagens de ambientação, ingredientes e oficina.

As imagens usam o atributo alt com uma descrição.

Vídeo

O vídeo está no arquivo video.html.

Foi usada a tag video com controls e um source apontando para:

media/videojapao.mp4

Tabela

O cronograma foi montado com uma tabela no arquivo cronograma.html.

Usei table, tr, th e td para mostrar dia, horário, atividade e responsável. A tabela foi usada só para os dados do cronograma.

Lista

No arquivo cardapio.html usei uma lista com ul e li para mostrar bebidas e acompanhamentos.

Formulário

O formulário está em contato.html.

Nele usei form, campos input, textarea e button para fazer um pedido de inscrição.

4.2 CSS

O CSS do projeto está separado no arquivo:

css/estilo.css

Seletores

No CSS usei seletores por tag, classe e id.

Alguns exemplos:

tag: body, h1, h2, h3, p, th, td e button;
classe: .logo, .secao, .atividade, .prato, .foto-galeria;
id: #principal, #cabecalho, #menu e #rodape.

Também usei seletor de atributo em:

input[type=text]

E combinação de tag com classe em:

a.link-menu

Links e pseudo-classes

No menu usei estilos diferentes para os links:

a.link-menu:link;
a.link-menu:visited;
a.link-menu:hover.

Também usei :hover em .botao-link:hover.

Cascata e herança

No body defini a fonte e a cor principal do texto, então essas configurações são usadas pelos elementos dentro da página.

Depois alguns elementos recebem estilos próprios. Por exemplo, existe uma regra geral para p e outra mais específica para p.destaque, que muda cor, fundo, borda e outras propriedades.

Fontes

No body usei:

Arial, Helvetica, sans-serif

Nos títulos h1, h2 e h3 usei:

Georgia, Times New Roman, serif

Organização dos blocos

Para colocar alguns elementos lado a lado usei float.

Isso aparece, por exemplo, em:

.logo;
.titulo-cabecalho;
.imagem-ilustracao;
.texto-caixa;
.resumo-pagina;
.atividade;
.prato;
.foto-galeria;
.informacoes-contato;
.formulario-contato.

Para parar o efeito do float depois dos blocos usei a classe:

.limpar { clear: both; }

Modelo de caixa

Foram usados margin, padding e border em várias partes do CSS.

Por exemplo, essas propriedades aparecem no #principal, nas seções, nos blocos da programação, nos pratos, na galeria, no formulário e no rodapé.

Position

Na classe .selo usei:

position: relative

junto com left e top para ajustar a posição do aviso da página inicial.

Unidades

No CSS usei principalmente:

px para tamanhos fixos, bordas e espaçamentos;
% para larguras dos blocos e imagens;
em para alguns tamanhos de fonte.
Estrutura das pastas

A organização usada no projeto é esta:

semana_cultura_japonesa/
├── index.html
├── programacao.html
├── cronograma.html
├── cardapio.html
├── galeria.html
├── video.html
├── contato.html
├── README.md
├── css/
│ └── estilo.css
├── img/
│ └── imagens usadas nas páginas
└── media/
└── videojapao.mp4