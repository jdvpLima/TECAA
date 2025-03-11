---
date: 2018-10-06
title: Documentação fácil com Docsy
linkTitle: Introdução ao Docsy
description: "O tema Docsy, baseado no Hugo, permite que os criadores de projetos foquem na criação de conteúdo sem precisar se preocupar com o desenvolvimento do site."
author: Riona MacNamara ([@rionam](https://twitter.com/bepsays))
resources:
- src: "**.{png,jpg}"
  title: "Imagem #:counter"
  params:
    byline: "Foto: Riona MacNamara / CC-BY-CA"
---

**Este é um post comum que inclui uma imagem.**

Nos metadados iniciais de cada post, estão o título, a data e um resumo, que é exibido na lista de postagens.


## Incluindo uma imagem

Aqui está uma imagem (`featured-sunset-get.png`) com byline e legenda.


{{< imgproc sunset Fill "600x300" >}}
Redimensionando uma imagem no Hugo 0.43
{{< /imgproc >}}


Os seguintes metadados, definidos no post, serão aplicados a todas as imagens deste post:

```
resources:
- src: "**.{png,jpg}"
  title: "Image #:counter"
  params:
    byline: "Photo: Riona MacNamara / CC-BY-CA"
```

Para adicionar uma imagem a uma página, use a seguinte configuração:

```
{{< imgproc sunset Fill "600x300" >}}
Redimensionando uma imagem no Hugo
{{< /imgproc >}}
```
As imagens serão exibidas com o tamanho e a byline especificados.