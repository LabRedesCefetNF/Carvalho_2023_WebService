# Carvalho_2023_WebService

## Resumo
Com o aumento do e-commerce, os mais diversos tipos de golpes virtuais são propagados pela Internet. 
Nem sempre é fácil decidir se uma loja é ou não segura para efetuar compras online. 
Portanto, é ideal que o usuário possua ferramentas para verificar a legitimidade de um site. 
Diante disso, este trabalho apresenta uma abordagem de identificação de dados administrativos em sites de e-commerce com TLD (top-level domain) .BR.
Para validar a proposta foi desenvolvida uma extensão de navegador que cruza os dados de pessoa jurídica com os dados do registro do domínio.
Com isso, o trabalho espera contribuir com a decisão dos usuários sobre sites de e-commerce.
 
Para atender às solicitações da extensão, foi desenvolvida esta API que requisita dados dois WebServices especializados.
Os dados dos domínios são obtidos por um servidor público https://registro.br/rdap/ do Registro.br, o departamento do NIC.br responsável pelas atividades de registro e manutenção dos nomes de domínios.
Os dados administrativos são obtidos por um serviço gratuito https://developers.receitaws.com.br/ da ReceitaWS, uma empresa que oferece uma API para obtenção de dados de pessoas jurídicas, advindos diretamente da Receita Federal.
A implementação focou especificamente em domínios .COM.BR. Uma vez, de posse dos dados de CNPJ, endereço, conta responsável, telefone, criação e validade do domínio, estes são comparados com os dados de inscrição, situação, telefones de contato, e-mail e endereço do Cadastro Nacional de Pessoa Jurídica. 
