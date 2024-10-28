# Projeto de Página de Login Responsiva
Este projeto implementa uma página de login simples e responsiva com HTML e CSS usando Tailwind CSS. A página apresenta campos de email e senha, opções de "lembrar-me" e "esqueceu a senha", além de botões para login social com Facebook e X.

## Funcionalidades
- **Formulário de Login**: Campos de email e senha com placeholders animados e um botão de envio.
- **Lembrar-me**: Checkbox para o usuário manter a sessão ativa.
- **Esqueceu a Senha**: Link de recuperação de senha.
- **Login Social**: Botões personalizados para login com Facebook e X.

## Pré-requisitos
- **Tailwind CSS**: A estilização utiliza classes do Tailwind CSS. Certifique-se de que `output.css` está gerado e referenciado corretamente.

## Estrutura do Projeto

- `index.html`: Estrutura HTML da página de login.
- `output.css`: Arquivo CSS gerado pelo Tailwind para aplicar as estilizações.
- `tailwind.config.js`: Configuração do Tailwind CSS para incluir estilos em todos os arquivos HTML e JS na pasta `src`.

## Como Utilizar
1. **Instalar Tailwind CSS**: Execute `npm install -D tailwindcss` para adicionar o Tailwind ao seu projeto.
2. **Gerar CSS**: Use `npx tailwindcss -i ./src/style.css -o ./output.css --watch` para gerar o arquivo `output.css`.
3. **Visualizar a Página**: Abra `index.html` em seu navegador para visualizar a página de login.

## Estrutura do Código
1. **Cabeçalho HTML**:
   - Inclui meta tags para charset e viewport e um link para `output.css`.
   
2. **Corpo HTML**:
   - **Seção Principal** (`<section class="h-screen">`): Área que cobre a tela inteira.
   - **Coluna Esquerda**: Contém uma imagem ilustrativa.
   - **Coluna Direita**: Formulário de login com campos de email e senha, opções de lembrar-me, links para redefinição de senha e login social.

## Exemplo de Código

```html
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./output.css" rel="stylesheet">
</head>
<body class="bg-violet-400">
  <section class="h-screen">
    <div class="container h-full px-6 py-24">
      <div class="flex h-full flex-wrap items-center justify-center lg:justify-between">
        <div class="mb-12 md:mb-0 md:w-8/12 lg:w-6/12">
          <img src="https://tecdn.b-cdn.net/img/Photos/new-templates/bootstrap-login-form/draw2.svg" class="w-full" alt="Phone image" />
        </div>
        <div class="md:w-8/12 lg:ms-6 lg:w-5/12">
          <form>
            <!-- Email input -->
            <div class="relative mb-6" data-twe-input-wrapper-init>
              <input type="text" class="peer block min-h-[auto] w-full rounded border-0 px-3 py-[0.32rem] leading-[2.15] outline-none transition-all duration-200 ease-linear focus:placeholder:opacity-100 peer-focus:text-primary" id="exampleFormControlInput3" placeholder="Email address" />
              <label for="exampleFormControlInput3" class="pointer-events-none absolute left-3 top-0 mb-0 max-w-[90%] origin-[0_0] truncate pt-[0.37rem] leading-[2.15] text-neutral-500 transition-all duration-200 ease-out peer-focus:-translate-y-[1.15rem] peer-focus:scale-[0.8] peer-focus:text-primary">Email address</label>
            </div>
            <!-- Password input -->
            <div class="relative mb-6" data-twe-input-wrapper-init>
              <input type="password" class="peer block min-h-[auto] w-full rounded border-0 px-3 py-[0.32rem] leading-[2.15] outline-none transition-all duration-200 ease-linear focus:placeholder:opacity-100 peer-focus:text-primary" id="exampleFormControlInput33" placeholder="Password" />
              <label for="exampleFormControlInput33" class="pointer-events-none absolute left-3 top-0 mb-0 max-w-[90%] origin-[0_0] truncate pt-[0.37rem] leading-[2.15] text-neutral-500 transition-all duration-200 ease-out peer-focus:-translate-y-[1.15rem] peer-focus:scale-[0.8] peer-focus:text-primary">Password</label>
            </div>
            <!-- Remember me checkbox -->
            <div class="mb-6 flex items-center justify-between">
              <div class="mb-[0.125rem] block min-h-[1.5rem] ps-[1.5rem]">
                <input class="relative float-left -ms-[1.5rem] me-[6px] mt-[0.15rem] h-[1.125rem] w-[1.125rem] appearance-none rounded-[0.25rem] border-[0.125rem] border-solid border-secondary-500 outline-none" type="checkbox" value="" id="exampleCheck3" checked />
                <label class="inline-block ps-[0.15rem] hover:cursor-pointer" for="exampleCheck3">Remember me</label>
              </div>
              <a href="#!" class="text-primary focus:outline-none">Forgot password?</a>
            </div>
            <!-- Submit button -->
            <button type="submit" class="inline-block w-full rounded bg-primary px-7 pb-2.5 pt-3 text-sm font-medium uppercase leading-normal text-white shadow-primary-3 transition duration-150 ease-in-out hover:bg-primary-accent-300">Sign in</button>
            <!-- Divider -->
            <div class="my-4 flex items-center before:mt-0.5 before:flex-1 before:border-t before:border-neutral-300 after:mt-0.5 after:flex-1 after:border-t after:border-neutral-300">
              <p class="mx-4 mb-0 text-center font-semibold">OR</p>
            </div>
            <!-- Social login buttons -->
            <a class="mb-3 flex w-full items-center justify-center rounded bg-primary px-7 pb-2.5 pt-3 text-center text-sm font-medium uppercase leading-normal text-white" style="background-color: #3b5998" href="#!" role="button">Continue with Facebook</a>
            <a class="mb-3 flex w-full items-center justify-center rounded bg-info px-7 pb-2.5 pt-3 text-center text-sm font-medium uppercase leading-normal text-white" style="background-color: #55acee" href="#!" role="button">Continue with X</a>
          </form>
        </div>
      </div>
    </div>
  </section>
</body>
</html>
