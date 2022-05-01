<h1> Utilização de API's </h1>

Os requisitos de layout são os mesmos da Atividade 1 e deve haver todas as funcionalidades que foram solicitadas. Nesta atividade iremos evoluir o projeto.

Nos projetos que estão sendo disponibilizados, já tem exemplos de como realizar post (no cálculo do IMC) e get (para montar a lista de estados). Estes serão os verbos http que iremos utilizar nesta atividade.

 

<h2>Regras do envio do formulário de cadastro:</h2>

 

A validação dos campos deve ser realizada pela API.<br><br>
Caso ocorra um erro com o status 422, os inputs devem ficar com borda vermelha e deve ser escrito abaixo do campo o motivo do erro do input afetado. O motivo do erro deve ser o que é retornado da API.<br><br>
Caso ocorra um erro com o status 4xx (exceto 422) ou 5xx e houver mensagem de erro “message”, está deve ser exibida ao usuário.<br><br>
Caso o erro do input seja corrigido, ao enviar o formulário, o input não deve mais ficar com borda vermelha e as mensagens devem ser apagadas.<br><br>
Caso dê sucesso no envio do formulário e tenha uma mensagem de resposta “message”, esta deve ser apresentada ao usuário.<br><br>
Quando o usuário entrar com o CEP, deve buscar o endereço pela API de endereço que consulta o CEP. Se retornar endereço, deve preencher com o resultado o “Logradouro”, “Estado” e “Cidade”. Caso de erro, não deve apresentar o erro ao usuário.<br><br>
Formulário só pode ser enviado se aceitar os termos.<br><br>
Após envio do formulário, campos devem ser "resetados" e botão de envio desabilitado até que o termo seja aceito novamente.<br><br>
