# <img src="https://www.linea.org.br/brand/linea-symbol.svg" alt="Logo LIneA" width="30 " height="30"> 2MASS Data Workflow Details

## 📤 Origem dos Dados
Baixar os arquivos com extensão **.gz** da tabela **PSC** do [`2MASS`](https://irsa.ipac.caltech.edu/2MASS/download/allsky/)


## 📥 Destino dos Dados 1
Path: /lustre/t1/public/2mass/*.gz

> OBS: Verificar Permissões: ***root:public???***


## 📥 Destino dos Dados 2
PostgreSQL
> OBS: baixar e ingerir no banco catalog_dev somente uma pequena amostra para validar que o pipeline funciona

**uri:** desdb4.linea.org.br

**db:** catalog_dev

**db schema:** twomass

**tabela:** psc

**user:** ***informar pelo slack***

**pass:** ***informar pelo slack***

Colunas a indexar com índice espacial Q3C:
  - ra
  - decl

Colunas a indexar (b-tree):
  - coadd_key
  - coadd


### [🔗 Schema da Tabela](https://irsa.ipac.caltech.edu/2MASS/download/allsky/twomass_psc_schema)

### [🔗 Validação dos Dados (somente em Produção)](https://irsa.ipac.caltech.edu/2MASS/download/allsky/verification_query_psc.html)

## References

[🔗 Data Workflow Details - IDAC 2MASS]( https://docs.google.com/document/d/1ovQOV9nlWSyL3Q9pmo40D1VcOiMYAvayURGdFJYhKf0/edit?usp=drive_link)

[🔗 https://irsa.ipac.caltech.edu/2MASS/download/allsky/README_ftp.html](https://irsa.ipac.caltech.edu/2MASS/download/allsky/README_ftp.html) 

[🔗 https://irsa.ipac.caltech.edu/data/2MASS/docs/releases/allsky/doc/sec1_4.html#ftpdes](https://irsa.ipac.caltech.edu/data/2MASS/docs/releases/allsky/doc/sec1_4.html#ftpdes) 

[🔗 https://drive.google.com/file/d/14uGig3Cwjz3xNl0IXCWSZ44W4FB5GFg9/view?usp=drive_link](https://drive.google.com/file/d/14uGig3Cwjz3xNl0IXCWSZ44W4FB5GFg9/view?usp=drive_link ) 
