# 🧵 Ateliê de Bordado — Catálogo Digital — Para acessar as funcionalidades abra o arquivo admin.html 

Site estático para catalogar seus desenhos de bordado, hospedável gratuitamente no **GitHub Pages**.

## Estrutura de Arquivos

```
bordado-site/
├── index.html              ← Site principal
├── data/
│   ├── categories.json     ← Categorias (editado pelo site)
│   ├── designs.json        ← Metadados dos bordados (editado pelo site)
│   ├── images/             ← Coloque aqui as imagens dos bordados
│   └── files/              ← Coloque aqui os arquivos (PDFs, etc.)
└── README.md
```

## Como usar

### Configurar no GitHub Pages
1. Crie um repositório no GitHub (pode ser privado ou público)
2. Faça upload de todos os arquivos deste projeto
3. Vá em **Settings → Pages → Source: main branch → /root**
4. Acesse `https://seu-usuario.github.io/nome-do-repo`

### Adicionar imagens e arquivos
Como o GitHub Pages é estático, imagens e arquivos são adicionados via Git:
1. Coloque imagens na pasta `data/images/`
2. Coloque arquivos (PDFs, padrões) na pasta `data/files/`
3. Faça commit e push
4. No site, ao criar um bordado, informe o caminho relativo (ex: `data/images/minha-rosa.jpg`)

### Salvar alterações (categorias e bordados)
O site edita tudo localmente e oferece botão para **exportar os JSONs**.
Após exportar, substitua `data/categories.json` e `data/designs.json` no repositório e faça commit.

### Dica: GitHub Desktop
Use o [GitHub Desktop](https://desktop.github.com/) para sincronizar sem usar a linha de comando.

## Funcionalidades
- ✅ Criar e apagar categorias com cores personalizadas
- ✅ Cadastrar bordados com nome, descrição, imagem e arquivo
- ✅ Apagar bordados individualmente
- ✅ Barra de pesquisa por nome/descrição
- ✅ Filtro por categoria
- ✅ Visualização em grade ou lista
- ✅ Exportar dados para sincronizar via Git
- ✅ Funciona em qualquer dispositivo com navegador
