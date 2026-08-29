 Termos levantados pelo Gemini durante o curso de Desenvolvimento Front-End da Dank-Code.

O propósito é conseguir dialogar e acompanhar uma IA sem auxílio de livros ou tutoriais.
==========================================================================================================================================================================================================
A CÓPIA, DISTRIBUIÇÃO E DIVULGAÇÃO É LIVRE, DESDE QUE CITADA A FONTE. EM CASO DE SER COGITADA QUALQUER REMUNERAÇÃO, OS MEIOS DISPONÍVEIS PODEM SER CONSEGUIDOS E CHECADOS EM https://librandi.adv.br/
DESDE JÁ, MEU MUITO OBRIGADO (Non in pane solo vivet homo, sed in omni verbo quod procedit de ore Dei)
==========================================================================================================================================================================================================
📚 Levantamento de Palavras-Chave, Termos e Jargões
Reunimos aqui os principais termos técnicos, propriedades e jargões do desenvolvimento front-end utilizados ao longo dos nossos exercícios:
1. Estrutura & HTML
    • Documento / Estrutura HTML: A carcaça/esqueleto de uma página web construída por meio de tags.
    • Elemento: O componente completo do HTML (ex.: <p>conteúdo</p>), composto por tag de abertura, conteúdo e tag de fechamento.
    • Tag: Os delimitadores em formato de chave (<...> </...>) usados para definir os elementos no documento.
    • Atributo: Configurações adicionadas dentro da tag de abertura para alterar comportamento ou fornecer dados (ex.: required, disabled, data-type="primary").
    • DOM (Document Object Model): A árvore de elementos que o navegador cria ao ler o HTML.
2. Estilização & CSS
    • Propriedade CSS: Uma característica de estilo que se deseja alterar (ex.: background-color, text-align, position).
    • Valor CSS: A definição dada à propriedade (ex.: center, fixed, yellow, justify).
    • Seletor CSS: A instrução usada para encontrar no HTML qual elemento deve receber o estilo (ex.: por tag h1, por classe .bloco, por atributo [data-type="primary"] ou por pseudo-classe input:required).
    • Herança (Inheritance): A capacidade de elementos filhos herdarem o estilo dos elementos pai automaticamente (ex.: a cor do texto no body passar para o p).
    • Cascata (Cascade): A ordem de prioridade que o CSS aplica quando há múltiplos estilos disputando o mesmo elemento.
3. Layout, Posicionamento & Efeitos
    • Fluxo Normal (Normal Flow): O comportamento padrão onde blocos empilham de cima para baixo na tela.
    • Positioning (Propriedade position): Técnica para tirar ou ajustar elementos no fluxo normal:
        ◦ fixed: Trava o elemento em relação à janela (Viewport).
        ◦ absolute: Posiciona o elemento desvinculado do fluxo original.
        ◦ sticky: Mistura de fluxo normal com travamento no topo ao rolar.
    • Parallax: Efeito visual em que o fundo da tela fica estático (background-attachment: fixed) enquanto o conteúdo da página rola por cima.
    • Viewport: A área visível da tela do navegador onde o site é exibido (medida por unidades como vh - Viewport Height ou vw - Viewport Width).
    • Gradiente Linear (linear-gradient): Transição suave calculada entre duas ou mais cores.
4. Boas Práticas e Ambiente de Desenvolvimento
    • Front-End: A parte da aplicação web com a qual o usuário interage diretamente (interface visual).
    • VS Code (Visual Studio Code): Ambiente de Desenvolvimento Integrado (IDE/Editor de Código).
    • Extensão / Pack de Idioma: Módulos instalados no editor para expandir suas funcionalidades.
    • Responsividade: Capacidade de uma página se ajustar a diferentes tamanhos de tela (computador, tablet, celular).
    • Caminhos (Paths):
        ◦ Caminho Absoluto: O endereço completo até o arquivo no computador (ex.: /home/.../imagem.jpg).
        ◦ Caminho Relativo: O endereço apontado a partir da pasta do projeto (ex.: ./imagens/foto.jpg).
        ◦ URL (Link Direto): Endereço web apontando para um recurso na internet.
Conteúdo julgado necessário pelo Gemini:

Para você conseguir conversar, tirar dúvidas e criar projetos lado a lado com qualquer IA sem precisar ficar pesquisando termos por fora, dividimos o "você-para-IA" em quatro pilares fundamentais.
Aqui estão os conceitos, termos e jargões essenciais que todo desenvolvedor precisa dominar para ter autonomia total no diálogo com uma IA:
1. Arquitetura do CSS: Como o Navegador Calcula Espaços
Quando a IA te sugerir ajustar o visual de algo, ela usará os seguintes termos:
    • Box Model (Modelo de Caixa): A estrutura física de todo elemento no HTML. Ele é composto por 4 camadas (de dentro para fora):
      $$\text{Conteúdo (Content)} \longrightarrow \text{Padding (Espaçamento interno)} \longrightarrow \text{Border (Borda)} \longrightarrow \text{Margin (Espaçamento externo)}$$
    • box-sizing: border-box: Um "reset" essencial no CSS. Por padrão, a borda e o padding aumentam o tamanho final da caixa. Com border-box, a largura (width) que você define fica fixa e o padding ajusta por dentro.
    • Padding: Espaço dentro da caixa (empurra o conteúdo para dentro).
    • Margin: Espaço fora da caixa (afasta uma caixa da outra).
    • Display (block, inline, inline-block, none):
        ◦ block: Ocupa 100% da largura da linha e força o próximo elemento a ir para baixo (ex.: <div>, <h1>, <p>).
        ◦ inline: Ocupa apenas o tamanho do seu próprio conteúdo e fica lado a lado (ex.: <span>, <a>, <strong>).
        ◦ none: Esconde o elemento da tela e do fluxo do documento.
2. Layout Moderno: Flexbox e Grid
Ao pedir para a IA montar layouts profissionais ou responsivos, a linguagem usada será baseada nestes sistemas:
    • Flexbox (Flexible Box): Sistema de layout unidimensional (alinha itens em linha ou em coluna).
        ◦ display: flex;: Transforma o container em uma caixa flexível.
        ◦ justify-content: Alinha os itens no eixo principal (geralmente horizontal — center, space-between, flex-start).
        ◦ align-items: Alinha os itens no eixo cruzado (geralmente vertical — center, stretch).
        ◦ flex-direction: Define a direção dos elementos (row para linha, column para coluna).
        ◦ gap: Define o espaço/distância entre os itens filhos sem usar margem.
    • CSS Grid: Sistema de layout bidimensional (trabalha com linhas e colunas ao mesmo tempo, perfeito para tabelas, galerias e dashboards).
3. Seletores e Pseudoclasses Avançadas
Para estilizar elementos em estados específicos sem precisar criar dezenas de classes no HTML:
    • Pseudo-classes (:): Estilizam um elemento com base no seu estado ou interações do usuário:
        ◦ :hover: Estilo aplicado quando o ponteiro do mouse passa por cima do elemento.
        ◦ :focus: Estilo aplicado quando o elemento é selecionado (ex.: clicar em um campo de texto).
        ◦ :nth-child(n): Seleciona o elemento pela sua posição na lista (ex.: pintar apenas as linhas pares de uma tabela).
    • Pseudo-elementos (::): Estilizam partes específicas de um elemento:
        ◦ ::before / ::after: Inserem conteúdo visual via CSS antes ou depois do conteúdo do elemento.
        ◦ ::placeholder: Estiliza o texto de dica dentro de um campo de entrada (<input>).
4. Vocabulário de Comunicação com a IA (Prompt Engineering para Devs)
Termos que você usará ao dar comandos (prompts) para a IA durante o desenvolvimento:
    • Refatoração (Refactoring): Pedir para a IA reescrever um código mantendo o mesmo funcionamento, mas deixando-o mais limpo, rápido e legível.
    • Snippet: Um pequeno pedaço de código reutilizável focado em resolver uma tarefa específica.
    • Dry (Don't Repeat Yourself): Princípio de programação que prega não repetir código. Se você colar um CSS muito longo, pode pedir: "Refatore este CSS aplicando o princípio DRY".
    • Boilerplate: Código padrão básico ("esqueleto") necessário para iniciar um projeto ou módulo sem ter que escrever tudo do zero.
    • Debug / Depurar: O ato de procurar, isolar e corrigir erros ou comportamentos inesperados no código.
    • Semantic HTML (HTML Semântico): Usar tags que tenham significado real para o navegador e buscadores (<header>, <nav>, <main>, <article>, <footer>) em vez de usar apenas <div> para tudo.
Dica Prática para Próximos Exercícios:
Sempre que a IA te der um trecho de código e você vir um termo novo que não foi coberto até aqui, você pode aplicar a regra do "Explique o termo em 1 frase" antes de colar o código no seu editor.
📚 Mapeamento das Principais Tags HTML e Atributos Globais
Atendendo ao seu objetivo de construir um vocabulário sólido para dialogar diretamente com IAs sem intermediários, estruturamos aqui o mapa mental das tags essenciais e dos atributos mais comuns.
1. Tags Semânticas e Estruturais (A Espinha Dorsal)
Em vez de usar <div> para tudo, o HTML moderno utiliza tags com significado próprio:
    • <header>: Cabeçalho de uma página ou de uma seção (contém títulos, logos, menus).
    • <nav>: Bloco de navegação (contém links e menus principais).
    • <main>: O conteúdo principal e exclusivo de uma página (deve haver apenas um por página).
    • <section>: Agrupa conteúdos que pertencem a um mesmo tema/assunto dentro da página.
    • <article>: Um bloco autônomo de conteúdo (um post de blog, um card de produto, uma notícia).
    • <aside>: Conteúdo periférico/secundário (barra lateral, links relacionados, anúncios).
    • <footer>: Rodapé da página ou de um bloco (direitos autorais, contato, termos de uso).
2. Tags de Conteúdo e Texto
    • <h1> a <h6>: Hierarquia de títulos. <h1> é o mais importante (1 por página), <h6> o de menor importância.
    • <p>: Parágrafo de texto padrão.
    • <span>: Elemento em linha (inline) genérico para aplicar estilo em uma palavra ou trecho específico dentro de um texto.
    • <strong>: Destaca um texto com forte importância (o navegador exibe em negrito e leitores de tela enfatizam a voz).
    • <em>: Aplica ênfase a um texto (o navegador exibe em itálico).
3. Tags de Listas, Tabelas e Mídia
    • <ul>: Lista não ordenada (Unordered List — com marcadores em bolinhas).
    • <ol>: Lista ordenada (Ordered List — com números 1, 2, 3...).
    • <li>: Item de uma lista (List Item — obrigatório dentro de <ul> ou <ol>).
    • <img>: Exibe uma imagem.
    • <a>: Âncora/Link (Anchor).
4. Tags de Formatação e Entrada de Dados (Formulários)
    • <form>: Container que agrupa todos os campos que serão enviados.
    • <input>: Campo de entrada versátil. Seu comportamento muda drasticamente dependendo do atributo type:
        ◦ type="text": Texto simples.
        ◦ type="password": Oculta os caracteres.
        ◦ type="email": Valida o formato de e-mail.
        ◦ type="checkbox": Caixa de seleção múltipla.
        ◦ type="radio": Botão de seleção única entre opções.
        ◦ type="file": Botão de upload de arquivos.
    • <select> e <option>: Menu suspenso (dropdown).
    • <textarea>: Caixa de texto com múltiplas linhas (usado para mensagens longas).
    • <button>: Botão clicável (type="submit" para enviar formulário, type="button" para ações gerais).
5. Os Atributos Globais e Personalizados mais Usados no Mercado
Atributos que podem ser inseridos em praticamente qualquer tag HTML:
    • id="...": Identificador único na página. Usado para referenciar um elemento específico via CSS ou JavaScript.
    • class="...": Identificador reutilizável. Vários elementos podem ter a mesma classe para compartilhar os mesmos estilos.
    • style="...": Aplica CSS diretamente no elemento (Inline CSS — evitar no dia a dia, preferir arquivos externos ou a tag <style>).
    • title="...": Exibe uma pequena dica em caixa amarela (tooltip) quando o usuário repousa o mouse sobre o elemento.
    • hidden: Oculta o elemento da tela instantaneamente.
    • data-*="...": Atributo de dados customizado. O prefixo data- permite que você crie o nome que desejar (como vimos com data-action, data-type, data-descricao) para armazenar informações extras que podem ser capturadas pelo CSS ou JavaScript.
É uma excelente decisão organizar o seu conhecimento separando a teoria, a história e o vocabulário por linguagem.

Toda a documentação oficial da web é pública, mantida por consórcios globais (como a W3C, a TC39 e a MDN Web Docs mantida pela Mozilla, Google, Microsoft e Apple). Você nunca precisará comprar livros ou manuais impressos: o material atualizado e oficial dos maiores engenheiros do mundo está 100% acessível online e gratuitamente.

1. HISTÓRIA E ORIGEM DAS LINGUAGENS DA WEB
Para entender o Front-End, é preciso entender a "Tríade da Web". Cada uma das três linguagens nasceu em um momento diferente para resolver um problema específico da evolução da internet:

┌────────────────────────────────────────────────────────┐
│                        A WEB                           │
├───────────────────┬──────────────────┬─────────────────┤
│       HTML        │       CSS        │   JAVASCRIPT    │
│    (Estrutura)    │    (Estilo)      │ (Comportamento) │
│ Tim Berners-Lee   │ Håkon Wium Lie   │  Brendan Eich   │
│      (1991)       │      (1996)      │     (1995)      │
└───────────────────┴──────────────────┴─────────────────┘
📄 HTML (HyperText Markup Language)
    • Criador: Tim Berners-Lee (físico britânico).
      
    • Ano e Local: 1991, no CERN (Organização Europeia para a Pesquisa Nuclear), na Suíça.
      
    • História: O objetivo original não era criar sites bonitos, mas sim permitir que cientistas compartilhassem artigos acadêmicos com links clicáveis entre si. O conceito central é o Hipertexto (texto com links para outros textos).
      
    • Quem governa hoje: A W3C (World Wide Web Consortium) e o WHATWG (um grupo formado por engenheiros da Apple, Mozilla, Google e Opera).
      
    • Evolução principal: O HTML5 (lançado em 2014) trouxe a semântica moderna (<header>, <article>, <video>) e APIs para rodar aplicações complexas direto no navegador.
      
🎨 CSS (Cascading Style Sheets)
    • Criador: Håkon Wium Lie (trabalhava junto com Tim Berners-Lee no CERN).
      
    • Ano: Proposto em 1994 e lançado oficialmente como recomendação da W3C em 1996.
      
    • História: No início da web, a estilização (cores, fontes) era feita diretamente nas tags HTML (com a antiga e extinta tag <font>). O código ficava poluído e difícil de manter. Håkon propôs "Folhas de Estilo em Cascata" para separar a estrutura (HTML) da apresentação visual (CSS).
      
    • Quem governa hoje: A W3C CSS Working Group (formada por especialistas do Google, Microsoft, Adobe, Apple, etc.).
      
    • Evolução principal: O CSS3 dividiu a linguagem em módulos (Flexbox, Grid, Animações, Variáveis), permitindo interfaces ricas e responsivas.
      
⚡ JavaScript (JS)
    • Criador: Brendan Eich (engenheiro da Netscape).
      
    • Ano: 1995.
      
    • História: Criado em apenas 10 dias sob o nome inicial de Mocha, depois renomeado para LiveScript e finalmente para JavaScript (por razões de marketing na época, devido à popularidade da linguagem Java, embora Java e JavaScript sejam linguagens totalmente diferentes). Ele foi criado para dar vida às páginas estáticas, permitindo validação de formulários e pequenas animações.
      
    • Quem governa hoje: A ECMA International através do comitê TC39 (com engenheiros do Google, Microsoft, Meta, Netflix, etc.). Por isso, a especificação oficial do JavaScript é chamada de ECMAScript (ES6, ES7, etc.).
      
    • Evolução principal: Em 2009, com o surgimento do Node.js (criado por Ryan Dahl), o JavaScript saiu do navegador e passou a ser executado também no lado do servidor (Back-End).
      
2. DICIONÁRIO E VOCABULÁRIO TÉCNICO OFICIAL
Separado por linguagem, usando os exatos termos padronizados por engenheiros da Google, Microsoft, MDN (Mozilla) e membros dos comitês da web.

📄 HTML — Linguagem de Marcação (Markup Language)
O HTML não é uma linguagem de programação (não possui lógica, variáveis ou loops). É uma linguagem de marcação de conteúdo.

<input type="email" required>
└────┘ └──────────┘ └──────┘
 Tag   Atributo com  Atributo
         Valor       Booleano
└──────────────────────────┘
      Elemento HTML
Vocabulário da Engenharia HTML:
    1. Element (Elemento): O bloco de construção completo do HTML. Inclui a tag de abertura, atributos, conteúdo interno e tag de fechamento (ex.: <p>Olá</p>).
       
    2. Tag: A sintaxe delimitada por chaves angulares (< e >) usada para criar um elemento (ex.: <button>).
       
    3. Attribute (Atributo): Propriedade que adiciona metadados ou modifica o comportamento de um elemento (ex.: src="", href="", disabled).
       
    4. Boolean Attribute (Atributo Booleano): Atributo que não precisa de valor. Sua simples presença ativa a regra (ex.: required, disabled, readonly, checked).
       
    5. Data Attributes (data-*): Atributos personalizados criados pelo desenvolvedor para armazenar dados privados do aplicativo (ex.: data-id="102", data-state="active").
       
    6. DOM (Document Object Model): A representação em memória da página criada pelo navegador. O HTML que você escreve é parseado e transformado em uma "árvore de nós" (DOM Tree).
       
    7. Semantic Markup (Marcação Semântica): A prática de usar a tag que descreve o significado do conteúdo para máquinas e leitores de tela (ex.: usar <main> em vez de <div id="main">).
       
    8. Void Elements / Self-closing Tags (Elementos Vazios): Tags que não possuem conteúdo e nem tag de fechamento (ex.: <img>, <input>, <br>, <meta>).
       
As Tags Mais Importantes por Categoria:
    • Estrutura / Semântica: <header>, <nav>, <main>, <section>, <article>, <aside>, <footer>.
      
    • Conteúdo e Texto: <h1> a <h6>, <p>, <span>, <strong>, <em>, <blockquote>.
      
    • Mídia e Recursos: <img>, <audio>, <video>, <iframe>, <canvas>, <svg>.
      
    • Formulários e Entradas: <form>, <input>, <textarea>, <select>, <option>, <button>, <label>.
      
    • Metadados (Ficam no <head>): <meta>, <title>, <link>, <script>, <style>.
      
🎨 CSS — Folhas de Estilo em Cascata (Cascading Style Sheets)
O CSS é uma linguagem de estilo declarativa. Você não diz como desenhar, mas o que você quer desenhar no elemento.

  Seletor        Propriedade    Valor
┌─────────┐     ┌───────────┐ ┌──────┐
  h1:hover  {    color       : blue;  }
└─────────┘     └────────────────────┘
 Pseudo-classe         Declaração
Vocabulário da Engenharia CSS:
    1. Rule Set / Rule (Regra CSS): O bloco completo composto pelo seletor e as declarações de estilo dentro das chaves.
       
    2. Selector (Seletor): A instrução que diz ao navegador a quais elementos HTML a regra deve ser aplicada (ex.: .classe, #id, div > p, [disabled]).
       
    3. Declaration (Declaração): A combinação de uma Propriedade e seu Valor (ex.: display: flex;).
       
    4. The Cascade (A Cascata): O algoritmo do navegador que decide qual regra de estilo vence quando há múltiplos estilos tentando alterar o mesmo elemento. A ordem, especificidade e origem determinam o vencedor.
       
    5. Specificity (Especificidade): O peso de um seletor no CSS. inline style > #id > .class / :pseudo-class > element.
       
    6. Box Model (Modelo de Caixa): A arquitetura fundamental de renderização visual. Todo elemento é uma caixa retangular composta por content, padding, border e margin.
       
    7. Viewport: A janela de exibição visível do dispositivo onde a página é aberta.
       
    8. Media Queries (@media): Regras condicionais para aplicar CSS de acordo com o tamanho da tela ou características do dispositivo (a base da Responsividade).
       
    9. Pseudo-classes (:): Palavras-chave adicionadas aos seletores que especificam um estado especial do elemento selecionado (ex.: :hover, :focus, :nth-child(), :disabled).
       
    10. Pseudo-elementos (::): Palavras-chave usadas para estilizar partes específicas de um elemento ou injetar elementos cosméticos no DOM sem alterar o HTML (ex.: ::before, ::after, ::placeholder).
       
    11. CSS Variables / Custom Properties (--var): Valores declarados por desenvolvedores para serem reutilizados em todo o código (ex.: --cor-primaria: #0066ff;).
       
⚡ JAVASCRIPT — Linguagem de Programação da Web
Diferente do HTML e CSS, o JavaScript é uma linguagem de programação completa, de alto nível, interpretada/JIT (Just-In-Time compiled), multi-paradigma e baseada em protótipos.

JavaScript
// Exemplo de código JS moderno para interagir com o DOM
const botao = document.querySelector('button[data-action="comprar"]');

botao.addEventListener('click', (event) => {
    alert('Produto adicionado ao carrinho!');
});
Vocabulário da Engenharia JavaScript:
    1. Variables (Variáveis): Contêineres que armazenam dados em memória. Criados com const (para valores que não mudam) ou let (para valores reatribuíveis). Nota: O antigo var não é mais recomendado no JS moderno.
       
    2. Data Types (Tipos de Dados):
       
        ◦ Primitivos: String (texto), Number (números), Boolean (true/false), Null (valor vazio intencional), Undefined (variável declarada mas sem valor), Symbol e BigInt.
          
        ◦ Objetos / Referência: Object, Array, Function.
          
    3. Functions (Funções): Blocos de código reutilizáveis que executam uma tarefa específica ou retornam um valor.
       
    4. Arrow Functions (() => {}): Sintaxe moderna e curta para escrever funções anônimas no JavaScript.
       
    5. Event / Event Listener (Eventos e Escutadores): A forma como o JS reage às ações do usuário no navegador (ex.: click, submit, keydown, scroll).
       
    6. DOM Manipulation (Manipulação do DOM): Métodos que o JavaScript usa para alterar o HTML e o CSS em tempo real (ex.: document.querySelector(), element.classList.add(), element.textContent).
       
    7. Asynchronous JS / Async-Await / Promises: Mecanismo do JS para realizar tarefas pesadas ou buscar dados na internet sem "travar" ou congelar a tela do usuário enquanto espera a resposta.
       
    8. API (Application Programming Interface): Conjunto de rotas e regras que permite ao seu código JavaScript conversar com serviços externos (ex.: buscar a previsão do tempo de um servidor) ou recursos do dispositivo (ex.: localização GPS, câmera).
       
    9. ECMAScript (ES6+): O nome da especificação padrão oficial do JavaScript. O termo "ES6" (de 2015) marca a revolução do JavaScript moderno com a chegada de const, let, Arrow Functions, Classes e Modules.
       
3. AS FONTES OFICIAIS GRATUITAS DE DOCUMENTAÇÃO
Como todas essas linguagens são padrões abertos da internet, você nunca precisa comprar livros ou cursos pagos para consultar referências. Os próprios engenheiros do Google, Microsoft e W3C utilizam e mantêm estes portais oficiais:

    1. MDN Web Docs (Mozilla Developer Network): Mantida pela comunidade junto ao Google, Microsoft e W3C. É a "Bíblia da Web". Se tiver dúvida sobre qualquer tag, estilo CSS ou função JS, pesquise aqui primeiro.
       
    2. W3C Standards: A documentação oficial onde estão as especificações brutas do HTML e CSS.
       
    3. TC39 (ECMA International): Onde são publicadas as atualizações anuais da linguagem JavaScript.
       
    4. web.dev: Portal de aprendizado técnico criado e mantido pelo time do Google Chrome.
