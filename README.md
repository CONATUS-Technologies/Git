# Guia de Referência de Comandos Git

Um guia para comandos Git e GitHub, abrangendo desde configurações básicas até fluxos de trabalho avançados.

## Sobre

Este repositório contém um material de referência completo para comandos Git, desenvolvido para auxiliar desenvolvedores de todos os níveis no uso efetivo de controle de versão. O guia apresenta explicações claras, exemplos práticos e melhores práticas para desenvolvimento profissional.

## Conteúdo

O guia está organizado em 12 seções principais:

1. **Comandos Básicos de Configuração** - Instalação e configuração inicial
2. **Iniciando um Repositório** - Criação e clonagem de repositórios
3. **Fluxo Básico de Trabalho** - Verificação de status, staging e commits
4. **Trabalhando com GitHub** - Conexão e sincronização com repositórios remotos
5. **Trabalhando com Branches** - Criação, mesclagem e gerenciamento de branches
6. **Histórico e Logs** - Visualização de commits e alterações
7. **Desfazendo Alterações** - Reversão de modificações e commits
8. **Arquivo .gitignore** - Configuração de arquivos ignorados
9. **Fluxo Completo de Trabalho** - Workflows passo a passo para diferentes cenários
10. **Comandos Úteis no VS Code** - Integração com Visual Studio Code
11. **Resolução de Problemas Comuns** - Soluções para erros frequentes
12. **Boas Práticas** - Diretrizes para desenvolvimento profissional

## Comandos Essenciais

### Configuração

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@example.com"
```

### Workflow Básico

```bash
git init                    # Inicializa repositório
git clone [url]             # Clona repositório
git status                  # Verifica status
git add .                   # Adiciona todos arquivos
git commit -m "mensagem"    # Faz commit
git push                    # Envia para GitHub
git pull                    # Baixa do GitHub
```

### Gerenciamento de Branches

```bash
git branch                  # Lista branches
git checkout -b [nome]      # Cria e muda para branch
git merge [nome]            # Mescla branch
```

## Características Principais

- Explicações detalhadas em português brasileiro
- Exemplos práticos para cada comando
- Padrões de workflow para diferentes cenários
- Seção dedicada à resolução de problemas
- Diretrizes de segurança e boas práticas
- Integração com VS Code
- Referências para recursos adicionais

## Público-Alvo

- Iniciantes aprendendo Git e controle de versão
- Desenvolvedores migrando de outros sistemas de controle de versão
- Equipes estabelecendo padrões de workflow com Git
- Profissionais que necessitam de referência rápida de comandos

## Estrutura do Documento

O documento foi desenvolvido para ser utilizado tanto como material de estudo linear quanto como referência rápida. Cada seção é autocontida e inclui:

- Sintaxe dos comandos
- Exemplos práticos de uso
- Explicação dos resultados esperados
- Observações importantes e avisos
- Casos de uso reais

## Workflows Incluídos

### Primeira Vez - Projeto Novo

```bash
git init
git add .
git commit -m "Primeiro commit"
git branch -M main
git remote add origin https://github.com/seu-usuario/seu-repo.git
git push -u origin main
```

### Fluxo Diário de Trabalho

```bash
git pull                              # Atualiza repositório
git status                            # Verifica alterações
git add .                             # Adiciona arquivos
git commit -m "Descrição do trabalho" # Salva localmente
git push                              # Envia para GitHub
```

### Feature Branch Workflow

```bash
git checkout -b feature/nova-funcionalidade
git add .
git commit -m "Implementa nova funcionalidade"
git push -u origin feature/nova-funcionalidade
```

## Resolução de Problemas

O guia inclui soluções detalhadas para:

- Erros de rejected (non-fast-forward)
- Conflitos de merge
- Problemas de autenticação
- Reversão de pushes indesejados
- Configuração de SSH e tokens de acesso

## Boas Práticas Destacadas

### Commits

- Faça commits pequenos e frequentes
- Cada commit deve representar uma mudança lógica
- Utilize mensagens claras e descritivas
- Sempre teste antes de commitar

### Branches

- main/master: código estável para produção
- develop: desenvolvimento em andamento
- feature/nome: novas funcionalidades
- bugfix/nome: correções de bugs
- hotfix/nome: correções urgentes

### Segurança

- Nunca commite senhas ou chaves de API
- Utilize .gitignore para arquivos sensíveis
- Use variáveis de ambiente (.env)
- Revise git status antes de cada commit

## Recursos Adicionais

O guia inclui links para:

- Documentação oficial do Git e GitHub
- Tutoriais interativos
- Guias de referência rápida
- Ferramentas de visualização

## Integração com VS Code

Inclui atalhos e comandos específicos para:

- Terminal integrado
- Interface Git nativa
- Extensões recomendadas (Git Graph, GitLens, GitHub Pull Requests)

## Licença

Para toda Humanidade.

---

**Nota**: Este é um guia de referência prático. Para documentação oficial completa, consulte [git-scm.com](https://git-scm.com/doc) e [docs.github.com](https://docs.github.com/).
