# EGWork - Site Corporativo

Site estático da EGWork desenvolvido com Jekyll e hospedado no GitHub Pages.

## Configuração do Ambiente

### Pré-requisitos
- Docker Desktop
- Visual Studio Code com extensão Dev Containers

### Desenvolvimento Local

1. Abra o projeto no VS Code
2. Quando solicitado, clique em "Reopen in Container" ou use o comando `Dev Containers: Reopen in Container`
3. Aguarde a configuração do ambiente (instalação do Ruby, Jekyll e dependências)
4. Execute o servidor local:
   ```bash
   bundle exec jekyll serve --host 0.0.0.0 --port 4000
   ```
5. Acesse o site em `http://localhost:4000`

### Estrutura do Projeto

```
├── _config.yml          # Configurações do Jekyll
├── _includes/           # Componentes reutilizáveis
├── _layouts/            # Templates de páginas
├── _sass/               # Estilos CSS
├── assets/              # Arquivos estáticos
├── .devcontainer/       # Configuração do Dev Container
├── CNAME                # Configuração do domínio personalizado
└── Gemfile              # Dependências Ruby
```

## Deploy

O site está configurado para deploy automático no GitHub Pages. Para fazer o deploy:

1. Faça commit das alterações
2. Push para a branch `main`
3. O GitHub Pages irá automaticamente fazer o build e deploy

## Domínio Personalizado

O domínio `egwork.com.br` está configurado no arquivo `CNAME`. Certifique-se de que o DNS do domínio aponte para o GitHub Pages.

## Comandos Úteis

```bash
# Instalar dependências
bundle install

# Servidor local
bundle exec jekyll serve

# Build do site
bundle exec jekyll build

# Limpar cache
bundle exec jekyll clean
```
