---
title: '2つの形式のPre-rendering'
date: '2020-01-01'
---

Next.jsには、**Static Generation**と**Server-side Rendering**の2つの形式のPre-renderingがあります。違いは、ページのHTMLを生成するときです。

- **Static Generation**は、**ビルド時**にHTMLを生成するPre-renderingメソッドです。Pre-renderingされたHTMLは、リクエストごとに_reused_されます。
- **Server-side Rendering**は、**各リクエスト**でHTMLを生成するPre-renderingメソッドです。


重要なことに、Next.jsでは、各ページに使用するPre-renderingフォームを**選択**できます。ほとんどのページでStatic Generationを使用し、他のページでServer-side Renderingを使用して、「ハイブリッド」Next.jsアプリを作成できます。