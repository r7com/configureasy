Configureasy
=============

A forma mais simples de carregar arquivos de configuração em suas Classe/Módulos.

##Instalação

Basta adicionar esta linha no seu Gemfile

```ruby
gem 'configureasy'
```

E entao executar:

    $ bundle

Ou instale manualmente:

    $ gem install configureasy

##Como usar

Basta incluir na classe e começar a usar

```ruby
class Foo
  include Configurable
end

Foo.config.some_key_in_config
# => 'some value for that key'
```

Por padrão ele busca um arquivo (.yml) no diretório _config_, caso precise especificar um nome diferente utilize o método _config_name_.

```ruby
class Foo
  include Configurable
  # load APP_ROOT/config/foo_config.yml
  config_name :foo_config
end
```

##Duvidas, questões e desconfianças em geral

mail me: ajfprates@gmail.com
