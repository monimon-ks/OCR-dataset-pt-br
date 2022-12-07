##(rascunho) Descrição do Dataset OCR para Português BR


### Origem dos Dados

- Amostras dos livros de Joaquim Nabuco e Machado de Assis foram coletadas no site dominiopublico.gov.br/

- Amostras de livros e publicações de diversos autores foram coletadas na Biblioteca Nacional Digital http://bndigital.bn.gov.br/

### Seleção dos textos

PDFs selecionados das obras de Joaquim Nabuco:
 -> "A carta abolicionista aos ingleses" (1985).
 -> "O abolicionismo" (1949)
 -> "Um estadista do império" (1949)

obras de machado de assis também são bem antigas e contém vocabulário antigo. 

fun fact:
 	existiram 4 frandes mudanças ortográficas na história do pt-br:
 	Reforma Ortográfica de 1911.
    	Formulário Ortográfico de 1943. (êle)
    	Reforma Ortográfica de 1971 (Brasil)
    	Acordo Ortográfico de 1990.


PDFs selecionados de livros/textos da biblioteca nacional digital:
 (obs: esses documentos possuem o ground truth nele mesmo pois é um pdf selecionável. Portanto precisaremos imprimir e escanea-los se forem a ser utilizados.)

  1 -> "Dürer — O Apogeu do Renascimento Alemão" páginas 7-28 (1999)

  2 -> " AUGUSTO DOS ANJOS UM TEMA PARA DEBATES" 30 páginas (1970)
  
  3 -> "Biblioteca Nacional Biografia" mais de 200 páginas com bastante texto por página e algumas imagens (1994)
  
  4 -> "BRASIL: RADIOGRAFIA DE UM MODELO" 180 páginas com folhas amarelas (1994)
  
  5 -> "História da imprensa no Brasil" 500 páginas (1983)


Documentos selecionados e seu total de páginas: 

   1 livro nabuco { "A carta abolicionista aos ingleses" } = 34

   5 livros acervo {todos} = 931
  
  =  **853 páginas (depois de tirar capas, sumários etc)**
  

### TO DO

  - [x] Selecionar número de páginas que extrairemos de cada documento. (feito, extrai todas páginas.)

  - [x] Extrair ground truth dos PDFs editáveis. 

  - [x] Transformar pdfs pesquisáveis para imagens-pdf. 
  
  - [ ] Fazer divisão de datasets (treino,valid e teste) por proporção de caracteres por sample. 



*Observações*:
  - escolhi páginas com texto puro, excluindo páginas que apenas imagens ou texto que contém algum formato diferente do texto puro (ex: tabelas, sumários, topicos).



