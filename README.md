# Repositório Público de Portfólio Profissional

Este repositório contém o código-fonte do meu portfólio profissional. O projeto foi desenvolvido para apresentar minhas habilidades, projetos e informações de contato de forma clara, moderna e responsiva.

## Visualização

Você pode visualizar o projeto finalizado [**clicando aqui**](https://eliaferreira.github.io/portifolio-elia/).

## Template Escolhido e Motivação

O template escolhido foi **Cover**, disponível no site oficial do **Bootstrap**.  
Motivos da escolha:

- **Layout Minimalista:** Estrutura de página única, limpa e focada no conteúdo.
- **Responsividade:** Adaptável a celulares, tablets e desktops.

## Customizações Implementadas

A partir do template original, implementei diversas alterações para criar uma identidade visual única e funcionalidades extras:

### 1. Definição de Nova Paleta de Cores

- **Tema Dark Mode:** fundo preto (`#000000`).  
- **Cor de destaque verde** (`#20c997`) aplicada em títulos, links, bordas e elementos interativos.

**Exemplo no CSS:**

```
body {
  background-color: #000000;
}
.main-title {
  color: #20c997;
}
```

### 2. Reestruturação do Layout Principal 

Layout em duas colunas em telas grandes: foto de perfil à direita, texto de introdução à esquerda.
Imagem de Perfil circular com borda e sombra verde.
Exemplo:

```
.profile-picture {
  width: 220px;
  height: 220px;
  border-radius: 50%;
  border: 3px solid #20c997;
  box-shadow: 0 0 25px 8px rgba(32, 201, 151, 0.5);
  transition: box-shadow 0.3s ease-in-out;
}
.profile-picture:hover {
  box-shadow: 0 0 35px 10px rgba(32, 201, 151, 0.7);
}
```

### 3. Galeria de Projetos

Seção "Projetos" criada do zero com cards do Bootstrap.
Cada card contém imagem padronizada e efeito de hover que aumenta o card e muda a cor da borda.
Exemplo:
```
.card {
  transition: transform .2s;
  border: 1px solid #20c997;
}
.card:hover {
  transform: scale(1.05);
  border-color: #28f5b2 !important;
}
.project-img {
  width: 100%;
  height: 160px;
  object-fit: cover;
}
```

### 4. Personalização de Botões e Links

Botão principal "Ver projetos" com fundo transparente e borda verde, mudando de cor ao passar o mouse.
Exemplo:

```
.btn-lg.border-custom-green {
  border: 2px solid #20c997;
  color: #fff;
  background-color: transparent;
}
.btn-lg.border-custom-green:hover {
  background-color: #20c997;
  color: #000;
}
```
Links de navegação com borda inferior verde em hover e estado active.

```
.nav-masthead .nav-link:hover,
.nav-masthead .active {
  border-bottom-color: #20c997;
  color: #fff;
}
```

### 5. Interatividade nos Ícones Sociais

Ícones do GitHub, LinkedIn e Instagram mudam de cor para verde ao passar o mouse.
```
.social-icon img:hover {
  transform: scale(1.2);
  filter: invert(67%) sepia(42%) saturate(1500%) hue-rotate(113deg);
}
```

### 6. Estilização do Formulário de Contato
Campos do formulário com tema escuro, borda verde e efeitos de foco.

```
.contact-form-container {
  border: 1px solid #20c997;
  padding: 1.5rem;
}
.form-control:focus {
  border-color: #31ebb4;
  box-shadow: 0 0 0 0.25rem rgba(36, 224, 168, 0.4);
}
```

### Tecnologias Utilizadas

- HTML5
- CSS3
- Bootstrap 
- Visual Studio Code

