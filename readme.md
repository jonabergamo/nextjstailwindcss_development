# Desenvolvimento front end utilizando Next.js e Tailwind css

![](https://github.com/jonabergamo/apresentacao2rp/blob/master/imagens/imagem%2001.jpg?raw=true)

## Requisitos Funcionais

- Node.js na versão v18.18.2 ou superior [https://nodejs.org/en/download]
- Git versão 1.8.5.2 ou superior [https://git-scm.com/downloads]

### Ambiente de Desenvolvimento Integrado (IDE)

- Recomendamos o uso do VSCode ou PyCharm, na versão mais recente.

### Sistema Operacional (SO)

- O projeto foi testado e é compatível com Windows e Linux.

## Requisitos Não Funcionais

### Conhecimentos Necessários

- Javascript ou Typescript: Conhecimento básico é recomendado.
- React.js: Conhecimento básico é necessário.
- CSS: Conhecimento básico é necessário.
- Node.js: Conhecimento básico é suficiente.
- Git: Conhecimento básico é necessário.

## Conceitos iniciais

O Next.js é um framework JavaScript de código aberto que funciona em conjunto com o React para facilitar o desenvolvimento de aplicações web. Ele oferece uma camada adicional de abstração sobre o React, fornecendo funcionalidades extras para construir aplicativos web de forma eficiente.

![](https://github.com/jonabergamo/apresentacao2rp/blob/master/imagens/Group%203078.png?raw=true)

Já o Tailwind CSS é um framework de estilo para a construção de interfaces de usuário em projetos web. Ao contrário de outros frameworks CSS que oferecem componentes pré-construídos, o Tailwind CSS adota uma abordagem diferente, fornecendo uma série de classes utilitárias que você pode aplicar diretamente nos elementos HTML para estilizar sua interface.

![](https://github.com/jonabergamo/apresentacao2rp/blob/master/imagens/tailwind.png?raw=true)

# Comparação entre React com e sem Tailwind CSS

## **React sem Tailwind CSS**

Ao usar React sem Tailwind CSS, os estilos geralmente são aplicados por meio de arquivos CSS ou módulos CSS. Cada componente React pode ter seu próprio arquivo de estilo, e a estilização é realizada de forma mais tradicional.

### Exemplo:

```jsx
// Componente React sem Tailwind CSS
import React from "react";
import "./Button.css";

const Button = () => {
  return <button className="custom-button">Click me</button>;
};

export default Button;
```

```css
/* Arquivo Button.css */
.custom-button {
  background-color: #3498db;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.custom-button:hover {
  background-color: #2980b9;
}
```

## **React com Tailwind CSS**

Com Tailwind CSS, a estilização é realizada diretamente nos elementos JSX usando classes utilitárias. Isso elimina a necessidade de arquivos de estilo separados e permite uma abordagem mais declarativa.

### Exemplo:

```jsx
// Componente React com Tailwind CSS
import React from "react";

const Button = () => {
  return (
    <button className="bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-700">
      Click me
    </button>
  );
};

export default Button;
```

No exemplo acima, as classes como `bg-blue-500` (cor de fundo azul), `text-white` (cor do texto branca), `px-4` (padding horizontal), `py-2` (padding vertical) e `rounded` (bordas arredondadas) são fornecidas pelo Tailwind CSS.

## **Vantagens e Desvantagens**

### **React sem Tailwind CSS:**

**Vantagens:**

- Maior familiaridade para desenvolvedores acostumados com CSS convencional.

**Desvantagens:**

- Mais código e arquivos para gerenciar.
- Maior propensão a conflitos de estilo.
- O peso total dos arquivos CSS pode afetar negativamente o tempo de carregamento do site para o cliente final, impactando a experiência do usuário.

### **React com Tailwind CSS:**

**Vantagens:**

- Desenvolvimento mais rápido e menos código.
- Consistência na estilização com classes predefinidas.
- O Tailwind remove automaticamente todo o CSS não utilizado ao ser construído para produção, o que significa que seu pacote final de CSS é o menor possível. Na verdade, a maioria dos projetos que utilizam o Tailwind enviam menos de 10kB de CSS para o cliente.

### Sites que utilizam tailwind css em seu interior

1.  **Alibaba:**

    - **URL:** [Alibaba Cloud](https://www.alibabacloud.com/)
    - **Detalhes:** Alibaba Cloud, a divisão de computação em nuvem da Alibaba Group, utiliza Tailwind CSS em seu site.

2.  **GitHub:**

    - **URL:** [GitHub](https://github.com/)
    - **Detalhes:** GitHub, uma das maiores plataformas de desenvolvimento colaborativo, adotou Tailwind CSS em algumas partes de sua interface.

3.  **Trivago:**

    - **URL:** [trivago](https://www.trivago.com.br/)
    - **Detalhes:** Trivago, um popular motor de busca de hotéis, é conhecido por ter adotado Tailwind CSS em seu desenvolvimento web.

## Next.js como ferramenta

### Por que utilizar o next.js como framework React?

Utilizar o Next.js como framework React oferece diversas vantagens:

1.  **Desenvolvimento Rápido:** O Next.js simplifica o desenvolvimento avançado de aplicativos React, proporcionando recursos prontos para uso e um compilador próprio que acelera os tempos de construção.
2.  **Performance:** O Next.js permite pré-carregar dados no servidor, resultando em tempos de carregamento mais rápidos em comparação com aplicações React tradicionais.
3.  **Renderização e SEO:** Oferece pré-renderização, enquanto o React utiliza renderização no lado do cliente. A pré-renderização facilita estratégias eficazes de SEO, melhorando a classificação nos motores de busca.
4.  **Roteamento Estruturado:** O Next.js fornece um sistema de arquivos pré-definido para roteamento, simplificando a configuração de páginas em comparação com opções de bibliotecas de roteamento do React.
5.  **SEO Aprimorado:** A capacidade do Next.js de realizar renderização no lado do servidor (SSR) melhora as classificações de SEO, proporcionando uma experiência de usuário otimizada com tempos de carregamento eficientes.
6.  **Pré-renderização Avançada:** Oferece métodos avançados de renderização, incluindo Client-Side Rendering (CSR), Server-Side Rendering (SSR), Static Site Generation (SSG) e Incremental Static Regeneration (ISR).
7.  **Facilidade de Configuração:** O Next.js oferece opções de configuração automáticas e manuais, com a ferramenta CLI create-next-app agilizando a inicialização do projeto.
8.  **Navegação Otimizada:** Utiliza componentes de link personalizados para otimizar a navegação e pré-carregar dados em segundo plano, melhorando o desempenho da aplicação.

Em resumo, o Next.js é especialmente benéfico para projetos React que se beneficiam de pré-renderização, como lojas online, aplicativos de mídia social, sistemas de reserva de ingressos e plataformas de educação. Ele oferece uma experiência de desenvolvimento mais rápida, melhor desempenho e recursos avançados de renderização, tornando-o uma escolha sólida para projetos ambiciosos.

### Sites que utilizam Next.js em seu interior

1. **Hulu:**

   - **URL:** [Hulu](https://www.hulu.com/)
   - **Detalhes:** Hulu é um serviço de streaming de vídeo on-demand que usa Next.js para oferecer uma experiência de usuário rápida e moderna em sua plataforma web.

2. **Twitch:**

   - **URL:** [Twitch](https://www.twitch.tv/)
   - **Detalhes:** Twitch, a plataforma líder em transmissões ao vivo para gamers, utiliza Next.js em algumas partes de seu site para melhorar a performance e a experiência do usuário.

3. **TikTok:**

   - **URL:** [TikTok](https://www.tiktok.com/)
   - **Detalhes:** TikTok, a popular plataforma de mídia para vídeos curtos, usa Next.js para sua versão web, permitindo uma navegação rápida e eficiente.

4. **Auth0:**

   - **URL:** [Auth0](https://auth0.com/)
   - **Detalhes:** Auth0, um provedor de autenticação e autorização como serviço, utiliza Next.js em seu site para uma entrega de conteúdo otimizada e segura.

5. **Vercel:**
   - **URL:** [Vercel](https://vercel.com/)
   - **Detalhes:** Vercel, a empresa por trás do Next.js, naturalmente usa seu próprio framework em seu site, demonstrando as melhores práticas e a potência do Next.js.

### Como iniciar um projeto em Next.js

#### 1. Criar um novo projeto Next.js

```batch
npx create-next-app@latest
```

#### 2. Responder o questionário de configuração no terminal

```batch
√ What is your project named? ... my-next-tailwind-app  // Escolha um nome qualquer ou um "." para instalar na raiz.
√ Would you like to use TypeScript? ... Yes
√ Would you like to use ESLint? ... Yes
√ Would you like to use Tailwind CSS? ... Yes
√ Would you like to use `src/` directory? ... Yes
√ Would you like to use App Router? (recommended) ... Yes
√ Would you like to customize the default import alias (@/*)? ... No
```

Após o questionário as dependencias necessárias serão instaladas e o projeto será inicializado

```batch
[#########.........] | idealTree:projeto: timing idealTree:#root Completed in 41917ms
```

#### 3. Iniciar o servidor de desenvolvimento

Execute o seguinte comando para iniciar o servidor de desenvolvimento:

```batch
cd my-next-tailwind-app
npm run dev
```

Acesse `http://localhost:3000` no seu navegador para ver o seu projeto Next.js com Tailwind CSS em ação!

![enter image description here](https://github.com/jonabergamo/apresentacao2rp/blob/master/imagens/first_page.png?raw=true)

No React as páginas estáticas em HTML são geradas a partir de um arquivo .jsx para javascript ou .tsx para typescript, note o x no final das extensões de arquivo, simbolizando uma extensão de arquivo especial reservada para o desenvolvimento em React.

Navegando até `app/page.tsx`, é possivel observar uma estrutura semelhante a demonstrada a baixo, onde é possivel perceber o uso prático da estilização através do tailwind css.

```jsx
import Image from "next/image";

export default function Home() {
  return (
    <main className="flex min-h-screen flex-col items-center justify-center p-8">
      {/* Seção central com imagem do Next.js */}
      <div className="relative flex place-items-center mb-8">
        {/* Imagem do Next.js */}
        <Image
          className="dark:drop-shadow-[0_0_0.3rem_#ffffff70] dark:invert"
          src="/next.svg"
          alt="Next.js Logo"
          width={180}
          height={37}
        />
      </div>

      {/* Mensagem de boas-vindas */}
      <p className="text-center text-xl mb-8">
        Get started by editing{" "}
        <code className="font-mono font-bold">app/page.tsx</code>.
      </p>

      {/* Link para a documentação */}
      <a
        href="https://nextjs.org/docs?utm_source=create-next-app&utm_medium=appdir-template&utm_campaign=create-next-app"
        className="rounded-lg border border-transparent px-5 py-4 transition-colors hover:border-gray-300 hover:bg-gray-100 hover:dark:border-neutral-700 hover:dark:bg-neutral-800/30"
        target="_blank"
        rel="noopener noreferrer">
        <h2 className="mb-2 text-2xl font-semibold">
          Docs{" "}
          <span className="inline-block transition-transform motion-reduce:transform-none">
            -&gt;
          </span>
        </h2>
        <p className="m-0 text-sm opacity-70">
          Find in-depth information about Next.js features and API.
        </p>
      </a>
    </main>
  );
}
```

`* O código acima foi resumido para fins didáticos *`

## Criação de Rotas no Next.js

O Next.js utiliza um sistema de roteamento baseado em arquivos, o que significa que as rotas são definidas pela estrutura de arquivos no diretório `app`. Isso torna a criação e gerenciamento de rotas incrivelmente simples e intuitivo. Vamos ver como isso funciona na prática.

exemplo de rota: meusite.com.br/sobre/nosso-time

Utilizando o React padrão, a criação de rotas necessita da instalação da biblioteca react-router-dom e uma configuração manual. Para o Next.js, o sistema de roteamento já vem pré instalado e configurado no projeto, sendo possivel criar uma aplicação com ou sem roteamento, basta escolher a opção desejada ao iniciar o projeto com o `create-next-app@latest`.

### Estrutura Básica de Rotas

1.  **Página Inicial (`/`):**

    - Para definir a página inicial do seu aplicativo, você cria um arquivo chamado `page.jsx` (ou `page.tsx` se estiver usando TypeScript) dentro do diretório `app`.Lembrando que um componente deve estar iniciado dentro do arquivo.

    ```jsx
    // app/page.jsx

    export default function Page() {
      return (
        <>
          <h1>Página Inicial</h1>
        </>
      );
    }
    ```

2.  **Rotas Estáticas:**

    - Cada diretório com um arquivo `page` JS ou TSX dentro do diretório `app` representa uma rota estática. Por exemplo, criar `page.jsx` em `about` resulta na rota `/about`.

    ```jsx
    // app/about/page.jsx

    export default function Page() {
      return (
        <>
          <h1>Página Inicial</h1>
        </>
      );
    }
    ```

3.  **Rotas Dinâmicas:**

    - Para rotas dinâmicas, você usa colchetes para envolver o nome de um novo diretório na rota. Por exemplo, `posts/[id]` e dentro um arquivo `page.jsx`, resultando `/posts/1`, `/posts/2`, etc.

    ```jsx
    // pages/posts/[id].jsx

    function PostPage({ params }) {
      const { id } = params;

      return <div>Post ID: {id}</div>;
    }

    export default PostPage;
    ```

4.  **Rotas de 404:**

    É possivel utilizar da lógica de rotas dinâmicas para capturar rotas que não são existentes na página e exibir uma mensagem genérica, evitando erros na tela. Para fazer isso basta adicionar uma rota dinâmica junto com rotas estáticas.

    Para ilustrar, considere a seguinte estrutura no diretório pages da sua aplicação:

    - Um arquivo `page.jsx` que lida com a página raiz `(/)`.
    - Um diretório `[not_found]` contendo um arquivo `page.jsx`, projetado para capturar e tratar qualquer rota que não corresponda a outros arquivos ou diretórios específicos.

    ```jsx
    // app/[not_found]/page.jsx

    function NotFound({ params }) {
      const { not_found } = params;

      return <div>Página {not_found} não foi encontrada.</div>;
    }

    export default PostPage;
    ```

<hr>

# Quiz

<details>
  <summary><strong>Por que usar o Next.js?</strong></summary>

O Next.js facilita a construção de interfaces de usuário para a web, adicionando recursos sobre o React. Ele possui uma comunidade robusta, documentação sólida e está ganhando popularidade entre os desenvolvedores web front-end.

</details>

<details>
  <summary><strong>O React é melhor que o Next.js?</strong></summary>

Não, o React não é melhor que o Next.js. Os desenvolvedores devem escolher um framework com base no que funciona melhor para o projeto e suas prioridades. (Um site focado em SEO, por exemplo, pode se beneficiar do Next.js, pois reduz os tempos de carregamento da aplicação.)

</details>

<details>
  <summary><strong>Por que o Next.js é melhor que o React?</strong></summary>

O Next.js oferece velocidades de desenvolvimento aprimoradas, tempos de carregamento de aplicativos reduzidos e pré-renderização.

</details>

<details>
  <summary><strong>Qual é a diferença entre Next.js e React?</strong></summary>

Next.js é um framework React com funcionalidades adicionadas prontas para uso. React é uma biblioteca JavaScript comum usada para construir interfaces de usuário interativas, especialmente para aplicativos web.

</details>

<details>
  <summary><strong>Quais problemas o Next.js resolve?</strong></summary>

Next.js fornece pré-renderização e pode melhorar o desempenho de SEO com tempos de carregamento de aplicativos reduzidos.

</details>

<details>
  <summary><strong>Por que escolher o React.js?</strong></summary>

React é menos opinativo e mais estabelecido do que o Next.js, oferecendo aos desenvolvedores maior flexibilidade e recursos extensivos.

</details>

<details>
  <summary><strong>O React e o React.js são a mesma coisa?</strong></summary>

Sim, ambos os termos se referem à mesma biblioteca JavaScript.

</details>

<details>
  <summary><strong>O Next.js é um framework?</strong></summary>

Sim, o Next.js é um framework de código aberto baseado no React.

</details>

<details>
  <summary><strong>Por que usar o Tailwind CSS?</strong></summary>

O Tailwind CSS é uma ferramenta utility-first que oferece um conjunto amplo de classes predefinidas para estilização, proporcionando maior flexibilidade e controle sobre o design do seu projeto.

</details>

<details>
  <summary><strong>Quais são as vantagens do Tailwind CSS?</strong></summary>

- **Customização:** O Tailwind permite personalizar as classes para atender às necessidades específicas do seu projeto.
- **Produtividade:** A abordagem utility-first acelera o desenvolvimento, reduzindo a necessidade de escrever CSS personalizado.
- **Manutenção:** Classes padronizadas facilitam a manutenção do estilo em todo o projeto.

</details>

<details>
  <summary><strong>O que diferencia o Tailwind de outros frameworks CSS?</strong></summary>

- **Sem predefinições de estilo:** Ao contrário de alguns frameworks, o Tailwind não impõe estilos predefinidos, permitindo uma aparência única para cada projeto.
- **Configuração flexível:** A configuração é altamente ajustável, proporcionando controle total sobre as classes disponíveis.

</details>

<details>
  <summary><strong>Como posso personalizar o Tailwind para atender às necessidades específicas do meu projeto?</strong></summary>

Você pode personalizar o Tailwind ajustando o arquivo de configuração `tailwind.config.js`, onde é possível adicionar novas classes, configurar cores, fontes e muito mais.

</details>

<details>
  <summary><strong>O Tailwind é adequado para todos os projetos?</strong></summary>

Embora o Tailwind seja adequado para muitos projetos, sua abordagem utility-first pode ser mais vantajosa em projetos pequenos a médios. Em projetos maiores, a gestão de classes pode se tornar mais complexa.

</details>

<hr>

_Revisão Técnica:_ `Jonathan Oliveira Bergamo`

Links úteis para estudo:

- [https://daily.dev/blog/why-i-moved-from-styled-components-to-tailwind-css-and-whats-the-future-of-css-in-js]
- [https://blog.bitsrc.io/comparing-styled-components-and-tailwind-css-50cdc6ee1c6c]


