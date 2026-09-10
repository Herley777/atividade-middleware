# Atividade Laravel - Middleware

## Objetivo

Criar uma aplicação utilizando o Framework Laravel onde uma rota aciona uma Middleware responsável por verificar a permissão de acesso.

Quando o usuário não possui permissão, a Middleware bloqueia o acesso e apresenta a seguinte mensagem:

> Você não tem permissão para acessar este site.
>
> Favor entrar em contato com o administrador.

---

## Tecnologias utilizadas

- PHP
- Laravel
- HTML
- Blade
- Middleware
- Visual Studio Code

---

## Estrutura do projeto

### Controller

O Controller utilizado é o `SiteController`.

Arquivo:

`app/Http/Controllers/SiteController.php`

O método `index()` é responsável por chamar a página `site`.

```php
public function index()
{
    return view('site');
}

## Execução da Middleware

![Acesso Negado](PrintsDeExecuçãoMiddleware/acesso-negado.png)