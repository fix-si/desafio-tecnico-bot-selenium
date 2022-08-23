<h1 align="center">
  desafio técnico bot-selenium
</h1>

<p align="center">
  Desenvolver uma automação web seguindo o passo a passo abaixo <br>
  site: http://aplicativos.tjes.jus.br/corregedoria/atm/Default.aspx
</p>

## OBJETIVO DO DESAFIO
Implementar um programa que utilize web scraping para uma automação web no site já citado. Será necessário inserir alguns dados no site ao decorrer da execução, os dados estão disponibilizados em uma planilha, e devem ser lidos linha por linha. O programa deverá repetir o passo a passo para cada linha da planilha. 

<br>

### INPUT
Os dados necessários para a aplicação estão disponibilizadas num arquivo `.xlsx`
- o arquivo `dados.xlsx` está disponível neste repositório.
   - os dados do arquivo serão utilizados ao decorrer da execução do programa.
  

### WEB SCRAPING

Após iniciar o navegador e abrir o site, o bot deverá interagir com os elementos da página: <br> <br>
  *`btn`* > clicar > próximo <br>
  *`checkbox`* > selecionar > juros moratórios <br>
  *`btn`* > clicar > próximo <br>
  *`input`* > inserir valor da planilha; referência: coluna A "valor moeda" <br>
  *`select`* > selecionar opção > juros legais <br>
  *`input`* > inserir valor da planilha; referência: coluna B "data inicial" <br>
  *`input`* > inserir data atual, do dia. <br>
  *`btn`* > clicar > próximo

Após isso será gerado um arquivo que poderá ser baixado como .pdf <br>
Deverá ser feito o download do arquivo com extensão `.pdf`


### OUTPUT
#### download arquivo pdf
- criar uma pasta dentro do diretório do programa e definir essa pasta como download padrão.
  - todos os pdf's baixados deverão estar nessa pasta.
  - cada pdf deverá ser renomeado de acordo com o nome que está na planilha; referência: coluna C "nome"
    - exemplo: SILVA.pdf
- após finalizar a execução, a pasta deverá conter os pdf's renomeados da seguinte forma:
  
    ![image](https://user-images.githubusercontent.com/92794401/186238644-c7a8c615-f5cf-47b6-a5c3-879993a71404.png)

    
#### extrair dados pdf
- deverá ser extraído o dado: **valor geral** de cada pdf baixado. Segue imagem de como a informação **valor geral** se encontra no pdf

    ![image](https://user-images.githubusercontent.com/92794401/186241633-dd985818-8208-4094-9076-5ce6c05a1e49.png)


- após extrair, a informação deve ser escrita na coluna "valor total"(*coluna D*) da planilha

#### planilha
- a coluna "status"(*coluna E*) da planilha deverá ser preenchida pelo bot, após cada iteração deverá escrever "concluído" na linha correspondente da coluna status.
  - exemplo de como a planilha deverá ser retornada ao final da execução:
    ![image](https://user-images.githubusercontent.com/92794401/186237793-c8720b6a-1769-49b2-8468-98964fc21719.png)


### TOOLS

deverão ser utilizadas as seguintes ferramentas:

- [Python](https://docs.python.org/3/)
- [Selenium Framework](https://www.selenium.dev/documentation/webdriver/)


### RECOMENDAÇÕES
- Utilize a versão mais recente do Python
- Utilize o selenium a partir da versão 4
- Leia sobre a biblioteca [tabula](https://pypi.org/project/tabula-py/)


### CRITÉRIOS DE AVALIAÇÃO
- A descrição do projeto deve explicar todos os passos necessários para executá-lo
- Processo de desenvolvimento versionado via Git em um repositório público
- Apresentação das informações solicitadas de forma clara e objetiva
- Organização do código
- Performance

<br>

### Dúvidas / sugestão
Caso haja alguma dúvida ou sugestão sobre o teste, pode criar uma issue neste projeto.

<br> <br>

> Esse teste é público. Candidatos para vagas na FIX-SI devem responder este teste como parte do processo seletivo.

