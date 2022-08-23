<h1 align="center">
  desafio técnico bot-selenium
</h1>

<p align="center">
  Desenvolver uma automação web seguindo o passo a passo abaixo <br>
  site: http://aplicativos.tjes.jus.br/corregedoria/atm/Default.aspx
</p>

## Objetivo do desafio
Implementar um programa que utilize web scraping para uma automação web no site já citado. Será necessário inserir alguns dados no site ao decorrer da execução, os dados estão disponibilizados em uma planilha, e devem ser lidos linha por linha. O programa deverá repetir o passo a passo para cada linha da planilha. 

### INPUT
Os dados necessários para a aplicação estão disponibilizadas num arquivo `.xlsx`
- o arquivo `dados.xlsx` está disponível neste repositório.
   - os dados do arquivo serão utilizados ao decorrer da execução do programa.
  
  
### WEB SCRAPING

Após iniciar o navegador e abrir o site, o bot deverá interagir com os elementos da página: <br> <br>
  *btn* clicar > próximo <br>
  *checkbox* selecionar > juros moratórios <br>
  *btn* clicar > próximo <br>
  *input* inserir valor da planilha; referência: coluna A "valor moeda" <br>
  *select* selecionar opção > juros legais <br>
  *input* inserir valor da planilha; referência: coluna B "data inicial" <br>
  *input* inserir data atual, do dia. <br>
  *btn* clicar > próximo

Após isso será gerado um arquivo que poderá ser baixado como .pdf <br>
Deverá ser feito o download do arquivo com extensão `.pdf`

### OUTPUT
- criar uma pasta dentro do diretório do programa e definir essa pasta como download padrão.
  - todos os pdf's baixados deverão estar nessa pasta.
  
- cada pdf deverá ser renomeado de acordo com o nome que está na planilha; referência: coluna C "nome"
  - exemplo: SILVA.pdf


### TOOLS

deverão ser utilizadas as seguintes ferramentas:

- [Python](https://docs.python.org/3/)
- [Selenium Framework](https://www.selenium.dev/documentation/webdriver/)


### Critérios de avaliação
- Processo de desenvolvimento versionado via Git em um repositório público
- Apresentação das informações solicitadas de forma clara e objetiva
- Organização do código
- Performance

