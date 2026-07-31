# RS2 Educação

Painel estático de monitoramento das metas BAE e RS 2/PCJ para municípios do Maranhão e do Piauí.

## Arquivos da raiz

O Netlify publica o site a partir da raiz do repositório. Os arquivos principais são:

- `index.html`: página principal publicada no site.
- `painel_monitoramento_bae.html`: cópia do painel para acesso direto, se necessário.
- `netlify.toml`: configuração do deploy.
- `README.md`: orientações do projeto.

Não manter arquivo duplicado como `index.html.html`, porque isso pode confundir a atualização do painel.

## Configuração no Netlify

- Build command: deixar vazio.
- Publish directory: `.`
- Base directory: deixar vazio.

O arquivo `netlify.toml` deve conter:

```toml
[build]
  publish = "."
```

## Atualização atual

Data-base do painel:

- BAE: 31/07/2026
- PCJ: 30/07/2026

## Como atualizar pelo Git GUI

1. Abrir o Git GUI.
2. Abrir o repositório `C:\Users\dioha\workspace\RS2-EDUCACAO`.
3. Clicar em `Rescan`.
4. Clicar em `Stage Changed`.
5. Escrever uma mensagem de commit, por exemplo: `Atualiza painel BAE 31-07`.
6. Clicar em `Commit`.
7. Clicar em `Push`.

Depois do push, o Netlify deve iniciar um novo deploy automaticamente.
