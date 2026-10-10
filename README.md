# Nutri Bio — site para Vercel

Site estático responsivo, em português, sem dependências de instalação ou build. Inclui as fotos reais dos dois produtos enviados, fotos de cultivo, identidade verde e branca, catálogo, detalhes em modal, orientação de aplicação, espaço para feedbacks e formulário de contato.

## Publicar na Vercel

1. Extraia o ZIP. A pasta com `index.html` deve ser a raiz do projeto.
2. Suba os arquivos dessa pasta em um repositório GitHub.
3. Na Vercel, clique em **Add New > Project** e importe o repositório.
4. Framework Preset: **Other**. Root Directory: pasta que contém `index.html`. Nenhum comando de build ou instalação é necessário. O arquivo `vercel.json` já define a saída.
5. Clique em **Deploy**. Também é possível usar o CLI: execute `vercel --prod` na pasta do site.

## Preencher os dados oficiais

Edite `config.js` para inserir WhatsApp (país + DDD + número), telefone, e-mail, preços, condições de compra e informações técnicas. Não inclua dados bancários ou segredos nesse arquivo público.

O site funciona sem esses dados, mas o atendimento direto só é ativado quando existe um WhatsApp ou e-mail válido. Antes disso, o formulário prepara uma mensagem copiável e informa que não houve envio. Depois de configurar, ele abre WhatsApp ou e-mail para o visitante confirmar o envio. Não há caixa de entrada, envio automático, backend, armazenamento de leads, pagamento ou checkout.

Os preços são individuais para cada apresentação. `null` mostra “Preço sob consulta”. O catálogo está na página Produtos; o botão solicita informações pelo formulário.

## Conteúdo a validar antes do lançamento comercial

- História: não foram fornecidos fundação, datas, cidade, fundadores ou marcos. O texto institucional é uma proposta editorial de propósito, a aprovar pela empresa. Substitua pelo histórico oficial na seção `sobre` do `index.html`.
- Informações técnicas: descrição do biofertilizante sólido e aplicação foliar a 5% (500 ml para 10 L) fornecidas pelo solicitante. A orientação foi inserida no produto sólido. Como a embalagem é sólida e a medida informada é em ml, o preparo da solução deve ser confirmado com a equipe. Não foram fornecidos frequência, culturas nem instruções completas de preparo. As alegações de fermentação e ação mais rápidas foram fornecidas pelo solicitante; validar tecnicamente antes da divulgação.
- Depoimentos: não foram fornecidos relatos reais. A seção informa que as experiências ainda serão publicadas após validação e autorização. Não contém clientes, avaliações ou testes fictícios. Insira apenas depoimentos reais e autorizados.
- Contatos fornecidos: (41) 9629-7122 e cesar.stafim@escola.pr.gov. O número foi mantido exatamente como informado, sem acrescentar um nono dígito; WhatsApp configurado com o código do Brasil. Confirmar que o número possui WhatsApp e que o endereço de e-mail está correto. Preços e condições continuam pendentes.
- Identidade: símbolo vetorial de broto desenvolvido para o site; substitua pelo arquivo oficial da marca se disponível.
- Política de privacidade: revisar com os dados oficiais da empresa e de seu atendimento antes de operar comercialmente.

## Arquivos

- `index.html`: estrutura e textos.
- `styles.css`: aparência e adaptação para celular.
- `app.js`: menu, modais, catálogo e contato.
- `config.js`: dados comerciais e técnicos.
- `assets/`: imagens locais e símbolo. O site não depende de fontes ou imagens hospedadas em terceiros.
- `vercel.json`: configuração de publicação.

## Verificação

`npm run check` valida a sintaxe do JavaScript. Abra `index.html` para uma inspeção local. O uso de copiar mensagem exige HTTPS ou localhost; na Vercel existe HTTPS. Verificação visual em navegador não realizada no ambiente de criação, que não disponibilizou o controle de navegador requerido para essa etapa.

## Imagens

Produtos: fotos fornecidas pelo solicitante. Fotos editoriais de campo/cultivo: Unsplash, `photo-1500382017468-9049fed747ef` e `photo-1500937386664-56d1dfef3854`, baixadas para entrega independente. São imagens ilustrativas; não representam áreas ou testes da Nutri Bio. Referência de licença: https://unsplash.com/license.
