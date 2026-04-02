# FreeLancee

### Prosposta Feita com o intuito de uma atividade pratica ###

<img width="1914" height="939" alt="image" src="https://github.com/user-attachments/assets/c0248ca3-3452-4f95-ae02-00ee5fdcc2af" />

Para criar um excelente arquivo README.md no GitHub, é importante que a explicação seja organizada por camadas: estrutura, estilo e funcionalidade.

Aqui está uma proposta de explicação detalhada e estruturada para você copiar e colar:

💻 Sobre o Projeto: Simulador de Freelancer
Este projeto é uma aplicação web simples que simula uma plataforma de contratação de serviços de tecnologia. Ele permite que o usuário visualize diferentes categorias de especialistas, adicione serviços a um carrinho virtual e veja o cálculo do total em tempo real.

🛠️ Estrutura Técnica
O projeto foi construído utilizando o trio fundamental do desenvolvimento Web: HTML5, CSS3 (referenciado como style.css) e JavaScript.

1. Estrutura HTML (index.html)
O arquivo HTML está dividido em blocos semânticos para melhor acessibilidade e SEO:

<header> (Banner): Contém o título principal e uma barra de navegação com links para seções de serviços e suporte.

<main>: Onde reside o conteúdo principal, subdividido em:

Seção "Nossos Serviços" (#trabalhos): Utiliza divs com a classe .Servicos para cada card. Cada card contém uma imagem, título (H3), descrição, preço formatado e um botão de ação.

Seção "Pedidos" (#Pedido): Uma área dinâmica onde o JavaScript insere os itens selecionados em uma lista (<ul>) e exibe o valor acumulado.

Seção "Suporte": Espaço para contato e redes sociais.

<footer>: Rodapé com informações de direitos autorais e links de autoria (LinkedIn).

2. Lógica JavaScript (script.js)
O script é responsável pela interatividade da página e funciona da seguinte forma:

Mapeamento de Elementos: O código utiliza querySelectorAll e getElementById para identificar os botões de "Adicionar", a lista de pedidos e o visor do valor total.

Manipulação de Eventos: * Um loop forEach adiciona um "ouvinte de clique" (addEventListener) a cada botão de serviço.

Ao clicar, o script "sobe" para o elemento pai (parentElement) para capturar os dados específicos (nome e preço) daquele card.

Tratamento de Dados: * O preço é extraído como texto e convertido em um número decimal (parseFloat) após a limpeza de símbolos como "R$" e a troca de vírgulas por pontos via .replace().

Atualização do DOM:

Cria dinamicamente novos elementos <li> para a lista de compras.

Atualiza a variável global total e reflete esse valor na tela formatado com toFixed(2).

Finalização: O botão "Finalizar Pedido" dispara um alerta com o valor final e limpa a lista e o totalizador, resetando a interface para um novo uso.

🚀 Funcionalidades Principais
Seleção Dinâmica: Adicione múltiplos serviços sem recarregar a página.

Cálculo Automático: O sistema soma os valores de cada hora trabalhada instantaneamente.

Interface Responsiva: Preparado para diferentes tamanhos de tela (via meta tag viewport).

Feedback ao Usuário: Limpeza de carrinho e confirmação via alerta ao finalizar a compra.


