## Sobre o Repo.

- Esse repositorio possui toda a stack do zabbix que pode ser usada para ambientes de UAT e localmente. 

- Em tempo a mesma estrutura pode ser usada para pequenos ambientes produtivos ou como modelo para um ambiente de alto volume; **porém pontos especificos em relação a segurança e o uso de certificados de autoridade devem ser observados, assim como devidas ações de performance do banco de dados! **

### Passos após clonar o repo.

![](https://raw.githubusercontent.com/rafapil/Imagens/master/zbx_stack/zbx_stack_001.PNG)

**Localizar a estrutura principal**
###### Navegue até a pasta new-zabbix

![](https://raw.githubusercontent.com/rafapil/Imagens/master/zbx_stack/zbx_stack_002.PNG)

**Abra com seu Editor**
###### Caso queira ajustar alguma configuração especifica pode realizaar aqui, todos os arquivos necessários estão disponiveis.
###### Também é possivel ajustar o docker-compose para adicionar, melhorar ou mesmo subir a versão. (basta ajustar a imagem)

**Para executar e criar toda a stack use o camando: **
`docker-compose up -d `

Importante execute apartrir do mesmo diretorio que encontrasse o arquivo docker-compose.yaml, caso contrario será preciso adicionar o caminho. 

INFO. Caso queira destruir os containers/serviço após criar ou tenha realizado alguma modificação com erro, use o comando: 
`docker-compose down `

E faça os devidos ajustes, finalizando repita o comando anterior.

![](https://raw.githubusercontent.com/rafapil/Imagens/master/zbx_stack/zbx_stack_003.PNG)


**Conferindo o resultado da dashboard do docker**

![](https://raw.githubusercontent.com/rafapil/Imagens/master/zbx_stack/zbx_stack_004.PNG)

**Acessando**
Abra o navegador e entre com: 
`localhost:8081`

Credenciais padrão.
`user: Admin (sim é A em maiúscula)`
`senha: zabbix`

![](https://raw.githubusercontent.com/rafapil/Imagens/master/zbx_stack/zbx_stack_005.PNG)

**Finalizado! só utilizar**

![](https://raw.githubusercontent.com/rafapil/Imagens/master/zbx_stack/zbx_stack_006.PNG)
