<h1 align="center">Trabalho de Devops e UX - UniAlfa</h1>
<p align="center"><i>Repositório para versionamento e documentação do Trabalho do 3°período no 2°Bimestre de Devops e UX.</i></p>

# Projeto de Interface para Sistema de Internet

## Visão Geral

Este projeto visa o desenvolvimento de uma interface responsiva e estático (alguns elementos, funções e páginas não estarão disponíveis) para um sistema de internet, com as seguintes páginas:

1. Janela de Login
2. Tela de Recuperação de Senha
3. Tela de Cadastro de Novo Usuário
4. Tela Principal do Sistema

## Estrutura do Projeto

### Diretório Principal
- **index.html**: Página principal, é a home do projeto com uma base para ser colocadas notícias e propagandas posteriormente.
- **recuperar-senha.html**: Página para recuperação de senha.
- **cadastro.html**: Página para cadastro de novo usuário.
- **login.html**: Página de login.
- **css**: Pasta para guardar os arquivos CSS para estilização das páginas.

## Requisitos Básicos de cada página e regras de negócio de cada item (regras para serem adicionadas posteriormente)

### Janela de Login
- **Campos**:
  - Usuário ou E-mail:
    - Origatório
    - Deve ser cadastrado
  - Senha:
    - Origatório
    - Deve ser cadastrado
    - Deve ser condizente com o usuário
- **Botões e outros clicaveis**:
  - "Login" (redireciona para o index.html)
  - "Esqueci minha senha" (redireciona para a tela de recuperação de senha)
  - "Criar conta" (redireciona para a tela de cadastro do usuário)
- **Design**: Responsivo para diferentes tamanhos de tela.
- **Outros**: A logo do sistema deve ficar no header.

### Tela de Recuperação de Senha
- **Campos**:
  - E-mail:
    - Obrigatório
    - Deve estar cadastrado
    - Deve ser um email
- **Botão e links**:
  - "Redefinir Senha" (envia link de recuperação de senha para o e-mail e ativa uma mensagem)
  - "Precisa de Ajuda?" (envia para alguma forma de contato)
- **Mensagens**:
  - Confirmação de envio do e-mail (redireciona para a página de login)

### Tela de Cadastro de Novo Usuário
- **Campos**:
  - Nome completo:
    - Obrigatório
  - E-mail:
    - Obrigatório
    - Deve ter formato de email
  - Nome de usuário:
    - Obrigatório
    - Não pode já estar cadastrado
  - Senha:
    - Obrigatório
    - Pelo menos 8 caracteres
    - Pelo menos uma letra maiúscula
    - Pelo menos um número
    - Pelo menos um caractere especial
  - Confirmação de senha:
    - Obrigatório
    - Deve ser igual a senha acima
  - Aceitação de Termos (checkbox):
    - Termos de uso
    - Políticas de privacidade
- **Mensagens**:
  - Sucesso após envio do formulário após a validação (Enviar para a página de login)
  - Erro após envio do formulário após a validação
- **Botões**:
    - "Cadastrar" (Cadastrar usuário se tudo estiver certo e enviar a mensagem adequada)

### Tela Principal do Sistema
- **Elementos**:
  - Logotipo do Sistema (leva para o index.html)
  - Caixa de Texto para Busca (Deve fazer uma busca no banco de dados)
  - Ícone de Usuário [Leva para a página de perfil(não existe)]
  - Ícone de Menu (com opções de acessibilidade e navegação no site)
  - Recurso para Notícias/Propagandas (localização de onde devem ficar, com imagem e texto)
- **Design**: Uso de uma paleta de cores monocromática, responsivo e estético em diferentes dispositivos.

## Navegação entre páginas
- **Tela de Login** (login.html):
  - "Criar conta" -> cadastro.html
  - "Esqueci minha senha" -> recuperar-senha.html
  - "Login" -> index.html ou validações
  
- **Tela de Recuperar Senha** (recuperar-senha.html)
  - "Redefinir Senha" -> mensagem -> login.html
  - "Precisa de Ajuda?" -> forma de contato
  
- **Tela de Cadastro** (cadastro.html)
  - "Termos de Uso" -> termos de uso
  - "Política de Privacidade" -> política de Privacidade
  - "Cadastrar" -> mensagem sucesso -> login.html ou mensagem erro -> cadastro.html
  
- **Tela Principal** (index.html)
  - "Links de tópicos" -> para as páginas dos tópicos
  - "Logo" -> index.html
  - "Perifil" -> página de perfil ou login.html se não estiver cadastrado
  - "noticias" -> levam para as páginas da noticia

## Requisitos Técnicos

1. **Responsividade**: Interface funcional e estética em desktop, tablet e smartphone.
2. **Acessibilidade**: Possibilidade de modo escuro e possibilidade alterar o tamanho das letras.
3. **Usabilidade**: Interface intuitiva e fácil de usar.
4. **Design Visual**: Usando uma estética semelhante aos portais de notícia.

## Disponíveis no projeto

1. **Documentação do Projeto**: Encontrasse nesse arquivo de README
2. **Código Fonte**: HTML e CSS (com algumas poucas coisas em JS) com versionamento.

## Ferramentas e Tecnologias

- **HTML5**: Para a estrutura das páginas.
- **CSS3**: Para a estilização das páginas.
- **JS**: Para ações pontuais.
- **Git/GitHub**: Para controle de versão e colaboração.

## Plano de Implementação

### 1. Configuração do Ambiente
- Instalar ferramentas necessárias.
- Configurar repositório no GitHub.

### 2. Desenvolvimento das Páginas
- Criar estrutura HTML das páginas.
- Adicionar estilização com CSS.
- Garantir responsividade utilizando Media Queries.

### 3. Validação e Testes
- Testar a interface em diferentes dispositivos.
- Testar navegação entre páginas.

### 5. Revisão e Refinamento
- Revisar o design e usabilidade.
- Refinar com base em feedbacks.
