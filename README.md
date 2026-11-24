# Prompt mestre — redesign de site em um único arquivo HTML

Atue como designer de produto, especialista em UX/UI e desenvolvedor front-end. Analise o material fornecido e implemente o redesign como um site navegável em um único arquivo chamado index.html. A entrega deve abrir por duplo clique em um navegador moderno e permitir testar o fluxo principal sem instalar nada.

## Briefing

- Nome do site ou organização — [Guarda Municipal]
- Referência atual — [URL, capturas de tela, HTML existente ou descrição]
- Nicho — [loja virtual, comércio local, prestador de serviços, órgão público, instituição de ensino, portfólio ou outro]
- Público — [quem usa o site, o que precisa fazer e em qual contexto]
- Objetivo principal — [comprar, pedir orçamento, encontrar um serviço, consultar informações, inscrever-se ou outro]
- Escopo — [página inicial e fluxo principal, ou seções específicas]
- Identidade visual — [logo, cores, fontes, referências e estilo desejado]
- Conteúdo confirmado — [produtos, serviços, contatos, preços, horários, textos e links]
- Imagens — [anexe as fotos e a logo autorizadas ou descreva os recursos disponíveis]
- Restrições — [o que precisa ser preservado e se recursos externos opcionais são permitidos]

Se eu informar apenas a URL, trabalhe na página inicial e no caminho até a ação prioritária. Se a URL estiver inacessível, use as referências fornecidas e diga brevemente o que ficou sem verificação. Tome decisões reversíveis para avançar quando o briefing estiver incompleto.

## 1. Entenda o público e reorganize a navegação

Identifique as três tarefas que o público mais precisa realizar. Revise a página atual, se estiver disponível, e corrija os pontos que dificultam essas tarefas, como rótulos vagos no menu, informação escondida ou etapas demais no celular. Preserve o conteúdo relevante, a identidade aprovada e o destino dos links confirmados.

Adapte a estrutura ao nicho e ao objetivo.

- Loja virtual — facilite encontrar produtos, comparar opções e revisar a seleção. Use busca, filtros e carrinho local quando fizerem sentido. Identifique o carrinho como demonstração se não houver checkout real.
- Comércio local — priorize produtos, cardápio ou serviços, horários, localização, rotas e canais de contato confirmados.
- Prestador de serviços — explique o que é oferecido, a quem e onde. Destaque a ação de pedir orçamento, agendar ou entrar em contato.
- Órgão público — organize o conteúdo por tarefas do cidadão. Priorize serviços, orientações e canais oficiais. Use linguagem simples e mostre requisitos, documentos e etapas somente com informação confirmada.
- Instituição de ensino ou evento — facilite consultar a programação, os requisitos, as datas e a inscrição.
- Portfólio — destaque trabalhos, contexto, contribuição e contato.

Para acomodar mais de uma seção no mesmo arquivo, use navegação por âncoras com IDs reais. Se o escopo for maior do que cabe em uma prévia executável, implemente o fluxo prioritário de ponta a ponta e indique as áreas que dependem das páginas originais.

## 2. Crie uma direção visual própria

Defina paleta, tipografia, espaçamentos e componentes de acordo com a marca. Dê uma função clara a cada seção. A primeira tela deve mostrar onde a pessoa chegou, o que pode encontrar e qual ação pode tomar. Escreva botões específicos, como “Ver serviços”, “Consultar horários” ou “Pedir orçamento”.

Comece pelo celular e refine o layout para tablet e desktop. Use grid ou flexbox, imagens proporcionais e largura de leitura confortável. Escolha uma composição adequada ao conteúdo. Use cartões quando ajudarem a comparar itens e listas quando facilitarem encontrar informações rapidamente.

Use as imagens autorizadas fornecidas. Quando houver acesso aos bytes, incorpore fotos otimizadas em data URI e use SVG inline para ícones ou ilustrações vetoriais adequadas. Sem os arquivos reais, use uma composição com tipografia, cor e formas. Adote fontes do sistema. Se eu autorizar recursos remotos opcionais, prepare uma alternativa local para que a página continue legível sem internet.

## 3. Implemente tudo no index.html

Use <!doctype html>, idioma adequado ao conteúdo, codificação UTF-8 e meta viewport. Inclua HTML semântico, CSS dentro de <style> e JavaScript nativo dentro de <script>, no fim de <body>. Mantenha no próprio arquivo os dados usados por busca, filtros, carrinho ou outros componentes locais.

A prévia deve funcionar em file:// sem servidor, instalação, compilação, frameworks, importações, CDN ou fetch de arquivos locais. Links confirmados para WhatsApp, mapas, páginas oficiais ou outros sites podem depender de internet. Mantenha a navegação e as interações da própria página utilizáveis sem conexão.

Faça cada controle cumprir a ação indicada. Use links com destino válido para navegação e botões para interações. Quando aplicável, implemente abertura e fechamento do menu móvel, busca, filtros, limpeza de filtros, estado sem resultados e validação de formulário. Use dados em memória por padrão. Se houver armazenamento local, trate a indisponibilidade sem interromper o uso.

Identifique claramente dados e fluxos de demonstração. Para recursos que exigem um backend, como envio de formulário ou checkout, implemente a parte local e explique na interface o que acontece ao interagir. Mensagens devem refletir o resultado real. Use apenas dados fornecidos ou confirmados para contatos oficiais, preços, prazos e depoimentos.

Inclua navegação por teclado, foco visível, alvos de toque confortáveis, contraste legível, texto alternativo para imagens informativas e rótulos associados aos campos. Se usar animações, respeite prefers-reduced-motion. Se usar um diálogo, permita fechá-lo com Escape e devolva o foco ao controle que o abriu.

## 4. Verifique e entregue o arquivo

Se houver um navegador disponível para teste, abra o arquivo pelo endereço file://. Confira o layout em larguras de 360, 768 e 1280 pixels, sem rolagem horizontal, e percorra o fluxo principal com mouse e teclado. Teste links internos, estados de erro e os controles que foram criados. Confira o console e repita o fluxo local sem internet. Se puder fazer apenas revisão do código, informe isso com precisão.

Entregue o index.html como arquivo baixável, quando a ferramenta permitir. Caso contrário, forneça todo o código em um único bloco marcado como html, de <!doctype html> a </html>, pronto para salvar como index.html em UTF-8. Inclua todas as partes da implementação, sem reticências ou trechos a completar. Feche com uma instrução curta para abrir o arquivo e mencione eventuais limitações de teste ou de integração.
