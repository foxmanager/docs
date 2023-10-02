# Como escrever um artigo

## O que é Markdown [^1]



> Arquivos Markdown tem a extensão .MD



Markdown é uma linguagem de marcação leve que você pode usar para adicionar elementos de formatação a documentos de texto simples. 

Em um aplicativo como o Microsoft Word, você clica em botões para formatar palavras e frases e as alterações ficam visíveis imediatamente. Markdown não é assim. Ao criar um arquivo formatado em Markdown, você adiciona sintaxe Markdown ao texto para indicar quais palavras e frases devem ter aparência diferente.

Por exemplo, para indicar um título, você adiciona uma "hashtag" antes dele (por exemplo, `# Título um`). Ou para deixar uma frase em negrito, você adiciona dois asteriscos antes e depois dela (por exemplo, `**isso é negrito**`). 

Você pode adicionar elementos de formatação Markdown a um arquivo de texto simples usando um aplicativo de edição de texto como o [Typora](https://typora.io) ou [Zettlr](https://zettlr.com).

O principal objetivo de design da sintaxe de formatação do Markdown é torná-la o mais legível possível. A ideia é que um documento formatado em Markdown possa ser publicado como está, como texto simples, sem parecer que foi marcado com tags ou instruções de formatação.

Abaixo um exemplo de Markdown renderizado:

<img src="_images/outros/dillinger.png" alt="Editor Markdown de Dillinger" style="zoom:30%;" />

## Sintaxe básica [^1]

### Títulos

| Marcação     | HTML                       |
| ----------------------- | -------------------------- |
| `# Título nível 1`      | `<h1>Título nível 1</h1>` |
| `## Título nível 2`     | `<h2>Título nível 2</h2>` |
| `### Título nível 3`    | `<h3>Título nível 3</h3>` |
| `#### Título nível 4`   | `<h4>Título nível 4</h4>` |
| `##### Título nível 5`  | `<h5>Título nível 5</h5>` |
| `###### Título nível 6` | `<h6>Título nível 6</h6>` |

 **Saída renderizada**

# Título nível 1

## Título nível 2

### Título nível 3

#### Título nível 4

##### Título nível 5

###### Título nível 6





### Formatação

\*itálico* = *itálico*

\**negrito** = **negrito**

\*\*\*negrito+itálico\*\*\* = ***negrito+itálico***

\==importante== = ==importante==

\`código\`= `código`

\~\~riscado\~\~ = ~~riscado~~

Texto \^sobrescrito^ = Texto ^sobrescrito^

Texto \~subescrito\~ = Texto ~subescrito~  

> **Atenção:** Não utilize espaços após os asteriscos.

###  Citações

> Citações são textos em blocos como esses.
>
> > Eles podem ser aninhados, com citações dentro de citações.
> >
> > Ou conter várias linhas.

Para aplicar uma citação, basta colocar o caractere '>' no início do bloco de texto.

\> Citação

(Renderizado abaixo) 

> Citação



### Listas

\- Basta incluir um hífen, e seguir com enter para os demais.

   \- Dois espaços, seguido de hífen ou um tab para um sub item. 

\1. Para listas numeradas, basta incluir um número seguido de um ponto.



- Basta incluir um hífen, e seguir com enter para os demais.
  - Dois espaços, seguido de hífen ou um tab para um sub item. 

1. Para listas numeradas, basta incluir um número seguido de um ponto.



> - Você também **pode** agregar vários elementos em um único parágrafo. 



### Links

Para um link como este: [FoxManager - Página principal](https://foxmanager.com.br).

Use: \[FoxManager - Página principal](https://foxmanager.com.br).

Você pode simplesmente colocar os link entre colchetes:

\<https://www.markdownguide.org>
\<mail@example.com>

Que serão renderizados assim:

<https://www.markdownguide.org>
<mail@example.com>

### 

Imagens

Para incluir imagens, o comando mínimo é:

\![]\(./_images/icon.svg)

> Entre os colchetes, coloque o caminho da imagem. 

![](./_images/icon.svg)

Para acrescentar um *hover* com mais detalhes da imagem, faça assim:

\![Um icone]\(./_images/icon.svg "Este é apenas um icone")

![Um icone](./_images/icon.svg "Este é apenas um icone")

Mais um exemplo:

\![daniel-cheung-sCdm5DiJb8w-unsplash]\(./_images/daniel-cheung-sCdm5DiJb8w-unsplash.jpg "Vem com o papai")

![daniel-cheung-sCdm5DiJb8w-unsplash](./_images/daniel-cheung-sCdm5DiJb8w-unsplash.jpg "Vem com o papai")

Agora a imagem com um link:

\[![Um icone]\(./_images/icon.svg "Icone com link para o FoxManager")]\(https://foxmanager.com.br)

[![Um icone](./_images/icon.svg "Icone com link para o FoxManager")](https://foxmanager.com.br)









### Linha Horizontal

Para acrescentar uma linha Horizontal como essa abaixo:

***

use \___ ou \---



### Itens de checagem
```
- [ ] Não checado
- [x] Checado
```
- [ ] Não checado
- [x] Checado



### Caractere de escape

Para exibir um caractere literal que de outra forma seria usado para formatar texto em um documento Markdown, adicione uma barra invertida ( `\`) na frente do caractere.




\\- Sem a barra invertida, isso seria uma lista.

Ou inicie um bloco com três crases (```)

```
O resultado será esse.
```



### Tabela

Abaixo um exemplo de tabela

```
| Cabeçalho 1 | Cabeçalho 2 |
| ----------- | ----------- |
| Linha 1     | Exemplo 1   |
| Linha 2     | Exemplo 2   |
```

O resultado será:

| Cabeçalho 1 | Cabeçalho 2 |
| ----------- | ----------- |
| Linha 1     | Exemplo 1   |
| Linha 2     | Exemplo 2   |


Você pode, ainda, alinhar o conteúdo das colunas das tabelas usando ---: onde os dois pontos, servem para dizer a direção do alinhamento.

```
| Cabeçalho 1 | Cabeçalho 2 |
| :---        | :---:       |
| Linha 1     | Exemplo 1   |
| Linha 2     | Exemplo 2   |
```

O resultado será:

| Cabeçalho 1 | Cabeçalho 2 |
| :--- | :---: |
| Linha 1     | Exemplo 1   |
| Linha 2     | Exemplo 2   |

### Notas de rodapé

Este é um exemplo de nota de rodapé[^1]ou talvez assim[^grande], basta apenas acrescentar isso \[^nota] que resultará em [^nota]

Para referenciar a nota de rodapé, acrescetente ao final do texto:

```
 [^nota]: Texto de exemplo
```















**Fontes:**

[^1]:  Markdown [Markdown.org] (https://www.markdownguide.org)
[^nota]: Aqui é apenas um exemplo do link de nota de rodapé.

