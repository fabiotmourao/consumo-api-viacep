## Como Usar

1. Clone o repositório para sua máquina local:

git@github.com:fabiotmourao/consumo-api-viacep.git

# Comportamento dessa consulta de endereço por CEP

Este repositório contém um código simples usando javascript html e css para que permite aos usuários consultar informações de endereço a partir de um CEP. 
O código utiliza a API pública do ViaCEP "https://viacep.com.br/ws/01001000/json/",
Para obter os detalhes do endereço correspondente ao CEP inserido pelo usuário no campo de entrada
O botão "Consultar CEP" tem evento onclick que acionaria uma função quando clicado.
Essa função obtem o valor do campo de entrada onde o usuário inseriu o CEP.
Em seguida, a função usa o método conecta() usando Fetch para fazer uma requisição à API https://viacep.com.br/ws/[campo de entrada]/json/,
substituindo por variavel ${cep} na URL.
Quando a resposta da API chegar, a função trará essa resposta. Se o CEP for válido, você receberia detalhes do endereço correspondente.
O resultado é então exibido na área designada da página.
