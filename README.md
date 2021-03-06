## PoliticosBR

[![Gem Version](https://badge.fury.io/rb/politicosbr.svg)](https://badge.fury.io/rb/politicosbr)

## Descrição

Esta gem fornece listas atualizadas de deputados e senadores brasileiros, com nome, partido, estado, período do mandato (apenas para os senadores), telefone e e-mail.

Se a sua aplicação tem como objetivo enviar mensagens para nossos "honestos e patrióticos" políticos, esta gem foi feita para você.

Ela é bastante simples e oferece apenas três métodos:

  * PoliticosBR.deputados
  * PoliticosBR.senadores
  * PoliticosBR.todos

Cada um desses métodos retorna uma array de hashes onde cada hash representa um deputado ou senador.

Assim, se tivermos:

```ruby
  arr = PoliticosBR.deputados
```

então para listar os nomes e e-mails de todos os deputados da lista podemos fazer

```ruby
  arr.each{ |dep|
    puts dep[:nome] + ' - ' + dep[:email]
  }
```

Os índices disponíveis no array são: **:nome**, **:partido**, **:estado**, **:mandato**, **:fones** e **:email**

## Coisas para fazer nas próximas versões

  * Selecionar deputados federais e senadores por estado
  * Deputados estaduais e distritais
  * Vereadores

## Autor

Edvaldo Silva de Almeida Júnior (EdDeAlmeidaJr)

  * e-mail:       edvaldoajunior@gmail.com
  * Skype:        edalmeidajr 
  * Celular:      +55-41-9507-3644
