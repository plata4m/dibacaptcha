# dibacaptcha
O projeto está organizado em 3 partes.  

1 - Em um diretório ficam imagens (.gif) que animam entre 5 e 7 imagens, sendo que na última aparecerá uma palavra, essa palavra será digitada no input.      
    
As imagens (.gif) que aparecem no captcha são apresentadas de forma randômica a cada acesso. Você pode criar seus próprios (.gifs), os do projeto são exemplos, mas funcionais.                  
    
Utilizamos um hash para nomear as imagens (.gif), pois a evolução da ferramenta é contínua, e num futuro as frases também terão hash.
    
2 - Um script de sua preferência como Java, Python, PHP no backend seleciona de forma randômica as imagens que aparecerão na interface. Nesse captcha utilizamos PHP para randomizar a apresentação.     

A frase que aparece nesse script PHP 'randomCaptcha.php' são as que deverão ser digitadas no input da interface para validação. Futuramente srá um hash também. Você também póde evoluir a ferramenta.   

3 - Na interface tem um serviço em JavaScript que chama o 'randomCaptcha.php' que por sua vez retorna uma imagem (.gif) randomica e a frase de validação, que será apresentada em uma DIV.                 

Essa frase é a que deverá ser digitada no input para validação.  Fizemos testes com log de acesso em um site que estava recebendo spam em um formulário de contato.  

Após colocar o captcha em um site que estava recebendo muitos spans através de seu formulário de contato, os envios de spans por robôs não ocorreram mais.  

Faça bom proveito. Manteremos sempre o projeto evoluindo com segurança e simplicidade.
