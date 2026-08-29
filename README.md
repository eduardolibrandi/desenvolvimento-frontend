 Termos levantados pelo Gemini durante o curso de Desenvolvimento Front-End da Dank-Code.

O propósito é conseguir dialogar e acompanhar uma IA sem auxílio de livros ou tutoriais. A presença de Inteligências Artificiais nas mais diversas profissões já não pode ser ignorada; e se ignorada não pode ser, então devemos nos adequar a ela.

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
