# Análise de dados administrativos de e-commerce: Uma abordagem focada no cliente

Com o aumento do e-commerce, os mais diversos tipos de golpes virtuais são propagados pela Internet. 
Nem sempre é fácil decidir se uma loja é ou não segura para efetuar compras online. 
Portanto, é ideal que o usuário possua ferramentas para verificar a legitimidade de um site. 
Diante disso, este trabalho apresenta uma abordagem de identificação de dados administrativos em sites de e-commerce com TLD (top-level domain) .BR.
Para validar a proposta foi desenvolvida uma [extensão de navegador](https://github.com/LabRedesCefetNF/Carvalho_2023_BrowserExtension) que cruza os dados de pessoa jurídica com os dados do registro do domínio.
Com isso, o trabalho espera contribuir com a decisão dos usuários sobre sites de e-commerce.
 
Para atender às solicitações da extensão, foi desenvolvida esta API que requisita dados dois WebServices especializados.
Os dados dos domínios são obtidos por um servidor público https://registro.br/rdap/ do Registro.br, o departamento do NIC.br responsável pelas atividades de registro e manutenção dos nomes de domínios.
Os dados administrativos são obtidos por um serviço gratuito https://developers.receitaws.com.br/ da ReceitaWS, uma empresa que oferece uma API para obtenção de dados de pessoas jurídicas, advindos diretamente da Receita Federal.
A implementação focou especificamente em domínios .COM.BR. Uma vez, de posse dos dados de CNPJ, endereço, conta responsável, telefone, criação e validade do domínio, estes são comparados com os dados de inscrição, situação, telefones de contato, e-mail e endereço do Cadastro Nacional de Pessoa Jurídica. 

# Realizar download do NODEJS <br>
# Siga o turorial abaixo conforme versão do sistema operacional antes de clonar o repositorio do GitHub. Lembrando que a versão do NodeJs deve ser acima da 14.<br>

<br>

# Linux *( testada na versão do Ubuntu 22.04.1 LTS )*

Utilize o passo a passo desse tutorial. https://computingforgeeks.com/how-to-install-node-js-on-ubuntu-debian/<br>
Prefira o *Method 2) Install Node.js and npm using NVM* do link acima ( METODO TESTADO E FUNCIONANDO )

# Windows *( Prefira a versão LTS sempre)*
Basta entrar no link e baixar a versão LTS <br>
    https://nodejs.org/en/download/


# Apos a instalação do NodeJs e o clonar o repositorio do GitHub, rodar os comandos abaixo no Visual Studio Code: <br>

* *npm init* <br>
* *npm i puppeteer*<br>
* *npm i node-fetch* -> site para conferencia ( https://www.npmjs.com/node-fetch ) <br>
* *npm i readline* -> site para conferencia ( https://www.npmjs.com/package/readline ) <br>
* *npm i fs* -> site para conferencia ( https://www.npmjs.com/package/fs ) <br>
* *npm i open* -> site para conferencia ( https://www.npmjs.com/package/open ) <br><br>

# Apos isso, faça a inserção do codigo abaixo conforme a imagem do repositorio *"imagem_config_package.png"*

    "type": "module"

# Apos isso, abrir o terminal do visual studio code ( https://code.visualstudio.com/download ) e digitar o codigo abaixo

    node index.js

<br><br>

Sites para conferencia dos repositorios utilizados do npm 

* *puppeteer -> site para conferencia (https://www.npmjs.com/package/puppeteer)*<br>
* *node-fetch* -> site para conferencia ( https://www.npmjs.com/node-fetch ) <br>
* *readline* -> site para conferencia ( https://www.npmjs.com/package/readline ) <br>
* *fs* -> site para conferencia ( https://www.npmjs.com/package/fs ) <br>
* *open* -> site para conferencia ( https://www.npmjs.com/package/open ) <br><br>
