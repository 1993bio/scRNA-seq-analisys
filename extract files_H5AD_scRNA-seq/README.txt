written in portuguese and also in english (bElow)

Para pesquisadores que tem em mãos seus arquivos H5Ad
e precisam separar os dados para análises mais robustas e
comparações mais robustas utilizar

obs: durante a montagem do andata criar o desing experimental dando um merge das tabelas
de paiente (controle) com ps pacientes (casos). Por exemplo juntar metadados de pacientes
tratados e controle em uma variavel, e depois juntar as contagens dos pacientes tratados
e controle em uma variavel e depois criar o objeto andata, para ter comparações de seu
intresse

passo a passo
Os dados utilizados neste pipeline é do estudo de Ziegler et al.2021.
epode ser obtido em:
- ZIEGLER, Carly GK et al. Impaired local intrinsic immunity to SARS-CoV-2 infection in severe COVID-19. Cell, v. 184, n. 18, p. 4713-4733. e22, 2021.

- https://www.covid19cellatlas.org/index.patient.html 

1º obter o arquivo H5AD:

2º Inicie o código "Extração de dados H5AD", e execute com o arquivo H5AD.

3º Inicie o código "juntar tabelas" e utilize os dados criados no código anterior.

4º Inicie o código " fatiamento de data frame" e selecione os dados que deseja pegar no 
In[46].

5º Inicie o código "separar contagens de metadados" este código separa os dados juntados anteriormente,
de modo que agora pode ser usado par criar o objeto anndata e H5AD para scanpy, ou para objetos Seurat.

6º Inicie o código "re-montagem do arquivo anndata e H5AD", faça seu design experimental, lendo os dados criados anteriormente
e atribuindo a variaveis distintas e junteos (como exemplificado no inicio deste documento). 
depois para iniciar o processo de criação do objeto anndata e exporte como .H5AD

Bonus: caso necessite renomear colunas para dar juntar tabelas ou etc.. utilizar o código "renomear colunas de tabelas"

############################################################################################################################

For researchers who have their H5Ad files in hand
and need to separate the data to
more robust comparisons.

obs: during the assembly of andata create the experimental design by merging the tables
of the patient (control) with the patient's feet (cases). For example, patient data
and control on one variable and then on the count of treated patients
and control in a variable and then create the adata object, to have comparisons of your
interest

step by step
The data used in this pipeline are from the study by Ziegler et al.2021.
and can be obtained from:
- ZIEGLER, Carly GK et al. Impaired local intrinsic immunity to SARS-CoV-2 infection in severe COVID-19. Cell, v. 184, n. 18, p. 4713-4733. e22, 2021.

- https://www.covid19cellatlas.org/index.patient.html

1st get the H5AD file:

2nd start the code "H5AD Data Extraction" and run it with the file H5AD.

3rd start the code "join tables" and use the data created in the previous code.

4th start the code "data frame slicing" and select the data you want to get in
In[46].

5th start the code "separate metadata counts" this code separates the data previously,
so now it can be used to create andata and H5AD objects for scanpy, or for Seurat objects.

6º start the code "andata and H5AD file reassembly", make your experimental design, reading the data created previously
and assigning to different variables and joining (as exemplified at the beginning of this document).
then to start the anndata object creation process and export as .H5AD

Bônus: caso precise renomear colunas para dar tabelas ou etc, use o código "rename columns de tables"