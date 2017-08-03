# watir_tips
Vamos mostrar os comandos do Watir Framework em Ruby.

### Para instalar o Watir, devemos enviar o comando abaixo para o cmd/shell/prompt do sistema:
```ruby
gem install watir-webdriver
```

### Após a instalação da biblioteca do Watir, devemos importar a biblioteca e instanciar o driver para poder usar as
### funções que o framework tem disponível.
```ruby
require 'watir-webdriver'
driver = Watir::Browser.new :firefox
```

### Para carregar a URL do Browser devemos usar a função "goto".
```ruby
require 'watir-webdriver'
driver = Watir::Browser.new :firefox # should open a new Firefox window
driver.goto 'http://nitrowriters.com/form/form.html'
```

### Para enviar um texto para um campo texto ou textarea devemos usar a função "set".
```ruby
driver.text_field(:id => 'my_text_field').set 'Yes!'
driver.textarea(:class => 'element textarea medium').set 'It was a long time ago, I do not remember'
```

### Watir pegar a localização de um elemento:<br>
location = browser.element(:id, 'id').wd.location<br>
puts "location x = #{location[0]}"<br>
puts "location y = #{location[1]}"


browser.textarea(:class, 'element textarea medium').focus



