# Corpus · Atlas anatômico em camadas

Atlas 3D de anatomia humana para estudantes de medicina, com corpos masculino e feminino, camadas, busca, fichas e casos clínicos interativos.

## Como publicar de graça no GitHub Pages

1. Crie uma conta em https://github.com (gratuita).
2. Clique em **New repository**, dê o nome `corpus` e marque **Public**. Clique em **Create repository**.
3. Na página do repositório, clique em **uploading an existing file**.
4. Arraste para a página **todo o conteúdo desta pasta**: todos os arquivos: `index.html`, `masculino.json`, `masculino.bin`, `feminino.json`, `feminino.bin`, `olhos-masculino.json`, `olhos-feminino.json`, `olho.jpg` e este `LEIA-ME.md`. Clique em **Commit changes**.
5. Vá em **Settings > Pages**. Em **Branch**, escolha `main` e a pasta `/ (root)`. Clique em **Save**.
6. Em um ou dois minutos o site fica disponível em `https://SEU-USUARIO.github.io/corpus/`.

## Como abrir no seu computador

Por segurança, os navegadores não carregam os modelos se você só der dois cliques no `index.html`. Para testar localmente, abra um terminal nesta pasta e rode:

```
python -m http.server 8000
```

Depois acesse http://localhost:8000 no navegador.

## Estrutura

- `index.html`: aplicação completa (interface, shaders, casos clínicos).
- `masculino.*` e `feminino.*`: malhas anatômicas em resolução completa, carregadas sob demanda.

## Créditos e licenças

- Corpos externos e olhos: gerados com o MakeHuman (makehumancommunity.org), licença CC0.
- Modelo masculino: BodyParts3D, © The Database Center for Life Science, CC BY 4.0. Malhas preparadas pelo projeto Human Atlas.
- Modelo feminino: Human Reference Atlas (HuBMAP), K. Browne e H. Schlehlein, baseado no Visible Human Female (U.S. National Library of Medicine), CC BY 4.0.
- Conteúdo educacional baseado em Moore, Netter, Guyton e Hall e no ATLS (10ª edição). Sujeito a revisão por professores e cirurgiões.
