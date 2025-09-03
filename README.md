# Landing Page PSN 

![Status do Projeto](https://img.shields.io/badge/status-concluído-green)
![Licença](https://img.shields.io/badge/license-MIT-blue)

Uma recriação conceitual e responsiva da página da PlayStation, desenvolvida com HTML5 e Bootstrap 5 e pronta para deploy com Docker e Nginx.

---
### Acesso ao Projeto (Live Demo)

O projeto está no ar e pode ser acessado através do GitHub Pages. Clique no botão abaixo para ver a aplicação em funcionamento:

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=github&logoColor=white)](https://analuisaabarbosa.github.io/landing-page-psn)

---

### Índice

* [Descrição do Projeto](#descrição-do-projeto)
* [Funcionalidades](#funcionalidades)
* [Tecnologias Utilizadas](#tecnologias-utilizadas)
* [Como Executar o Projeto](#como-executar-o-projeto)
* [Autor](#autor)

---

### Descrição do Projeto

Este projeto é uma landing page responsiva que demonstra a conversão de um design UI para um código HTML/CSS funcional.

A estrutura e o layout foram baseados em um protótipo de design para uma página de esportes, encontrado abertamente na comunidade do Figma. O desafio foi adaptar e remodelar completamente o tema original, aplicando uma nova identidade visual inspirada na **PlayStation Network (PSN)**.

O objetivo foi praticar habilidades de desenvolvimento front-end, focando na fidelidade a uma estrutura de design, na implementação da responsividade com Bootstrap 5 e na adaptação criativa de um tema. A aplicação é servida por um servidor web Nginx e está containerizada com Docker para simplificar o processo de deploy.

---

### Funcionalidades

- **Layout Responsivo:** A interface se adapta perfeitamente a qualquer tamanho de tela, graças ao sistema de grid do Bootstrap.
- **Componentes Modernos:** Utilização de componentes do Bootstrap 5 como Navbar, Carrossel de imagens, Cards.
- **Navegação Intuitiva:** Uma barra de navegação clara e funcional para uma ótima experiência do usuário.
- **Seções Bem Definidas:** Estrutura organizada com seções de destaque, novidades, jogos populares e rodapé informativo.
- **Pronto para Deploy:** Inclui um `Dockerfile` e a configuração do `Nginx` para um deploy rápido e consistente em qualquer ambiente que suporte Docker.

---

### Tecnologias Utilizadas

- **Front-end:**
  - `HTML5`
  - `Bootstrap 5`
  - `CSS3`
- **Servidor Web e Deploy:**
  - `Nginx`
  - `Docker`

---

### Como Executar o Projeto

Para executar esta aplicação localmente, você precisará ter o Git e o Docker instalados em sua máquina.

#### Pré-requisitos

- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/products/docker-desktop/)

#### Passo a Passo

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/analuisaabarbosa/landing-page-psn.git
    ```

2.  **Navegue até o diretório do projeto:**
    ```bash
    cd lading-page-psn
    ```

3.  **Construa a imagem Docker:**
    *Este comando irá ler o `Dockerfile`, baixar a imagem do Nginx e copiar os arquivos da sua aplicação para dentro da imagem.*
    ```bash
    docker build -t landing-page-psn .
    ```

4.  **Execute o contêiner a partir da imagem criada:**
    *Este comando inicia o contêiner em segundo plano (`-d`) e mapeia a porta 8080 do seu computador para a porta 80 do contêiner (`-p 8080:80`), onde o Nginx está rodando.*
    ```bash
    docker run -d -p 8080:80 landing-page-psn
    ```

5.  **Acesse a aplicação:**
    Abra seu navegador e acesse [http://localhost:8080](http://localhost:8080). Você deverá ver a landing page funcionando!

---

### Autor

Feito por **Ana Luisa**.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/analuisaabarbosa/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:analuisaaugustob@gmail.com)
