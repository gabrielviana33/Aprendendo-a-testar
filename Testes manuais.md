# Aprendendo a testar
Foi utilizado um site local para realização de testes: Central de atendimento ao Cliente

Este documento traz como aspectos mais importantes as seguintes abordagens sobre o site:


* Casos de teste. 
* Ferramentas de teste. 
* Modelos de teste. 
* Resultados de teste. 
* Subprodutos de teste. 
* Cobertura de teste. 

## Casos de teste

* Registrar Mensagem
* Consultar banco



## Ferramentas

Para esse projeto os testes foram realizados em uma máquina local com sistema opereacinal Windows 10 com acesso à internet e o aplicativo de captura de tela,o navegador Google Chrome(64-bits).

## Modelos

Seguem alguns dos exemplos realizados:



| Nº | Cenário | Localização | Pré-condição | Procedimento | Resultado esperado:
| ------------- |:-------------:| -----:| ------------- |:-------------:| -----:|
| 1 | Registrar mensagem | Tela Principal | Nome,sobrenome, e-mail e como posso ajudar? | Preencher: - nome - sobrenome - e-mail - como posso ajudar?<br/> Clicar: -enviar| Mensagem enviada com sucesso!. |
| 2  | Registrar e-mail invalido| Tela Principal | Nome, sobrenome, e-mail invalido e como posso ajudar? | Preencher: - nome - sobrenome - e-mail invalido e como posso ajudar? <br/> Clicar: -enviar | Indicar erro nos campos obrigatórios e não enviar mensagem. |
| 3 | Registra, em branco, inválido | Tela Principal | Sem pré condição | Clicar: -enviar | Indicar o erro e enviar mensagem. |
| 4 | Registro, poucos caracteres, inválido | Tela Principal | Nome, sobrenome, e-mail e telefone com menos de 11 caracteres | Preencher: - nome - sobrenome - e-mail - telefone - como posso ajudar?. <br/> Clicar: -enviar | Indicar o erro (poucos caracteres) e não enviar mensagem. |
| 5 | Registro, muitos caracteres, inválido | Tela Principal | Nome,sobrenome, e-mail, telefone com mais de 10 caracteres e como posso ajudar? | Preencher: - nome - sobrenome - e-mail - telefone com mais de 11 caracteres  <br/> Clicar: -enviar | Indicar o erro(excedeu caracteres) e não enviar enviar mensagem. |
| 6 | Clicar: Telefone (Tornando obrigatorio)  | Tela Principal | Nome,sobrenome, e-mail e como posso ajudar? | Nome,sobrenome, e-mail e como posso ajudar? <br/> Clicar: -enviar | Indicar o erro campos obrigatorios e não enviar mensagem. |


## Resultados

|N°|Resultado <br/> Esperado\|Obtido|  Sucesso  |Considerações|
| ------------- |:----------------:|:--------:| ------------- |
|1|Mesnsagem enviada com sucesso. <br/> \| <br/> Mesnsagem enviada com sucesso.|Sucesso ✅|
|2|Indicar erro nos campos obrigatórios e não enviar mensagem. <br/> \| <br/> Valide os campos obrigatorios. | Sucesso ✅|
|3|Indicar erro nos campos obrigatórios e não enviar mensagem. <br/> \| <br/> Valide os campos obrigatorios. | Sucesso ✅|
|4|Indicar o erro (poucos caracteres) e não enviar mensagem. <br/> \| <br/> Mesnsagem enviada com sucesso. | Falha ❌|
|5|Indicar o erro do usuário(excedeu numero de caracteres) e não  enviar mensagem. <br/> \| <br/> Mesnsagem enviada com sucesso. | Falha ❌|
|6|Indicar erro nos campos obrigatórios e não enviar mensagem. <br/> \| <br/> Valide os campos obrigatorios. | Sucesso ✅|


## Subprodutos
Os subprodutos tais como: scripts, imagens e vídeos resultados dos testes executados estão disponíveis neste repositório em suas respectivas pastas.
#### Imagens e vídeos relacionados aos casos de teste descritos neste documento possuem a numeração relacionada!


### Algumas gravações dos testes Manuais realizados:


[Gravações](https://github.com/gabrielviana33/Aprendendo-a-testar/tree/main/Videos)


[Registrar mensagem](https://github.com/gabrielviana33/Aprendendo-a-testar/blob/04327777e2b591962e86ffdf1a75e2039b270e9b/Videos/T1.webm)</br>
[Registrar e-mail invalido](Videos/T2.mp4)</br>
[Registra, em branco, inválido](Videos/T3.mp4)</br>
[Registro, poucos caracteres, inválido](Videos/T4.mp4)</br>
[Registro, muitos caracteres, inválido](Videos/T5.mp4)</br>
[Clicar: Telefone (Tornando obrigatorio)](Videos/T6.mp4)

## Cobertura

O nível de cobertura de testes é medido pela “%” porcentagem dos casos de teste executados com sucesso.

|Aceitação Completa |Acima de 95% dos casos de teste executados com sucesso!|O programa está pronto para o deploy!|
| ------------- |:----------------:|:--------:|
|Meio nível de aceitação|De 70 até 95% dos casos executados com sucesso|O programa pode ser liberado para o PO como um protótipo.|
|Inaceitável|Até 70% de casos executados com sucesso.|Qualidade insuficiente.|

##### O projeto atual se encontra com 66% dos seus testes executados com sucesso, o que o coloca em inaceitável!


<br/> 

