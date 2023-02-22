# Aprendendo a testar
Foi utilizado um site local para realização de testes: [Central de atendimento ao Cliente](file:///C:/workspace/cypress-basico-v2/src/index.html)

Para esse projeto o Documento que traz a abordagem completa utilizada é o: [Plano de teste!] e pode ser beixado para melhor vizualização.
Este documento traz como aspectos mais importantes as seguintes abordagens sobre o site:


* Casos de teste. 
* Ferramentas de teste. 
* Modelos de teste. 
* Resultados de teste. 
* Subprodutos de teste. 
* Cobertura de teste. 

## Casos de teste

* Registrar Mensagem
* Atualizar
* Consultar banco



## Ferramentas

Para esse projeto os testes foram realizados em uma máquina local com sistema opereacinal Windows 10 com acesso à internet e o aplicativo de captura de tela,o navegador Google Chrome(64-bits) e a ferramenta de captura de interações Katalon Recorder 5.5.3.

## Modelos

Porém, seguem alguns dos exemplos realizados:



| Nº | Cenário | Localização | Pré-condição | Procedimento | Resultado esperado:
| ------------- |:-------------:| -----:| ------------- |:-------------:| -----:|
| 1 | Registrar mensagem | Tela Principal | Nome,sobrenome, e-mail e como posso ajudar? | Preencher: - nome - sobrenome - e-mail - como posso ajudar?<br/> Clicar: -enviar| Mensagem enviada com sucesso!. |
|2  | Registrar e-mail invalido| Tela Principal | Nome, sobrenome, e-mail invalido e como posso ajudar? | Preencher: - nome - sobrenome - e-mail invalido e como posso ajudar? <br/> Clicar: -enviar | Indicar erro nos campos obrigatórios e não enviar mensagem. |
|3 | Registra, em branco, inválido | Tela Principal | Sem pré condição | Clicar: -enviar | Indicar o erro e enviar mensagem. |
|4 | Registro, poucos caracteres, inválido | Tela Principal | Nome, sobrenome, e-mail e telefone com menos de 11 caracteres | Preencher: - nome - sobrenome - e-mail - telefone - como posso ajudar?. <br/> Clicar: -enviar | Indicar o erro (poucos caracteres) e não enviar mensagem. |
|5 | Registro, muitos caracteres, inválido | Tela Principal | Nome,sobrenome, e-mail, telefone com mais de 10 caracteres e como posso ajudar? | Preencher: - nome - sobrenome - e-mail - telefone com mais de 11 caracteres  <br/> Clicar: -enviar | Indicar o erro do usuário(excedeu caracteres) e não cadastrar. |


## Resultados

|N°|Resultado <br/> Esperado\|Obtido|  Sucesso  |Considerações|
| ------------- |:----------------:|:--------:| ------------- |
|6|Indicar o erro do usuário(caractere inválido) e não cadastrar. <br/> \| <br/> Usuário criado com sucesso!|Falha ❌|
|7|Atualiza e carrega de novo a página. <br/> \| <br/> Atualiza e carrega de novo a página. | Sucesso ✅|
|8|Deleta o registro selecionado. <br/> \| <br/> Deleta o registro selecionado |Sucesso ✅|


## Subprodutos
Os subprodutos tais como: scripts, imagens e vídeos resultados dos testes executados estão disponíveis neste repositório em suas respectivas pastas.
#### Imagens e vídeos relacionados aos casos de teste descritos neste documento possuem a numeração relacionada!


### Algumas gravações dos testes Manuais realizados:


[registro com poucos caracteres nos campos de texto](https://user-images.githubusercontent.com/34687381/217560734-112be533-5d8f-406d-9d9d-e149dda3d3d5.webm)


[registro com campos em branco!](https://user-images.githubusercontent.com/34687381/217560563-8363b1fe-adec-4d1b-8751-fbd0d1883083.webm)


## Cobertura

O nível de cobertura de testes é medido pela “%” porcentagem dos casos de teste executados com sucesso.

|Aceitação Completa |Acima de 95% dos casos de teste executados com sucesso!|O programa está pronto para o deploy!|
| ------------- |:----------------:|:--------:|
|Meio nível de aceitação|De 70 até 95% dos casos executados com sucesso|O programa pode ser liberado para o PO como um protótipo.|
|Inaceitável|Até 70% de casos executados com sucesso.|Qualidade insuficiente.|

##### O projeto atual se encontra com 50% dos seus testes executados com sucesso, o que o coloca em inaceitável!


<br/> 

[//]: <> (Links)

[Plano de teste do projeto!]: https://github.com/lucas-dejard/Site-analise-2/blob/main/site%202%20-%20TestPlan.docx