# Formulários HTML

<div align="left">
 <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="40" alt="html5 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="40" alt="css3 logo"  />
</div>

###

> Repositório de aprofundamento sobre a entrada de dados por meio de formulários, arquivos das aulas do curso HTML Formação em Full-Stack – Mayk Brito Rodrigo Gonçalves.

</div>

## ✍️ Mini projetos

<p>Desenvolvi esses 2 pequenos projetos para praticar o aprendizado em aula</p>

<div align="left">

### Formulário de matrícula

<img src="./public/MacBook Pro-1735761452934.jpeg" alt="..." />
<img src="./public/MacBook Pro-1735761405609.jpeg" alt="..." />
<img src="./public/MacBook Pro-1735761410124.jpeg" alt="..." />
</div>

### 🔗 Deploy

<a href="https://html-forms-seven.vercel.app/">Confira aqui o projeto</a>

### Formulário de cadastro

<img src="./public/MacBook Pro-1735857904712.jpeg" alt="..." />
</div>

### 🔗 Deploy

<a href="https://html-forms-seven.vercel.app/">Confira aqui o projeto</a>


### Anotações 

**Sempre** devemos usar uma label para um input, seja ela oculta ou não, pois os leitores de tela não leem os placeholders.

<aside>
💡

**SEMPRE** usar a unidade de medida “rem” para as fontes, pois assim tornam elas responsivas de acordo com as configurações do navegador

</aside>

<aside>
💡

**SEMPRE** que o formulário tiver um input do tipo FILE, é necessário adicionar o atributo `enctype="multipart/form-data"` no elemento `<form>`

O atributo `enctype` especifica como os dados do formulário serão codificados ao serem enviados para o servidor. O valor `multipart/form-data` é necessário porque:

1. Permite enviar arquivos binários, como imagens, documentos ou vídeos, além de dados de texto.
2. Divide os dados do formulário em várias partes para que o servidor possa processar os arquivos e outros campos do formulário de maneira separada.

- Sem o atributo `enctype="multipart/form-data"`, o navegador enviará os dados do formulário usando a codificação padrão, `application/x-www-form-urlencoded`, que não suporta arquivos binários.
- Nesse caso, o arquivo não será enviado corretamente e você verá um erro ou comportamento inesperado no lado do servidor.
</aside>

<aside>
💡

**USO do :has**

```css
 &:has(input:focus) {
    border-width: 2px;
    border-color: var(--stroke-hightlight);
    background-color: var(--surface-secondary);

    & {
      color: var(--text-tertiary);
    }

    & svg path {
      stroke: var(--stroke-hightlight);
    }
  }
```

</aside>

<aside>
💡

**uso do :focus-within**

```css
input[type="date"]:focus-within {
  outline: 0.25rem solid var(--surface-primary);
  border: 0.125rem solid var(--stroke-hightlight);
  outline-offset: 0.1px;
}

// Essa pseudo classe serve para aplicar estilo caso algum elemento dentro desse 
elemento selecionado estiver em foco, nesse caso dentro do input[type="date"]
```

</aside>

