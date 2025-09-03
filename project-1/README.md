# Projeto: A Intersecção entre as Vias Metabólicas da Osteoporose e os Genes Alvos dos Medicamentos Raloxifeno, Ácido Zoledrônico e Alendronato de Sódio

# Descrição Resumida do Projeto

A osteoporose é uma doença osteometabólica caracterizada pela redução progressiva da densidade óssea e pela fragilidade estrutural do esqueleto, afetando cerca de 200 milhões de pessoas no mundo. Sua maior incidência ocorre em mulheres na pós-menopausa e em idosos, grupos nos quais o risco de fraturas representa importante impacto na qualidade de vida e nos custos de saúde. No Brasil, o envelhecimento populacional e o alto custo dos medicamentos reforçam a necessidade de estratégias terapêuticas eficazes e acessíveis.

O avanço das análises genômicas e bioinformáticas permite aprofundar a compreensão dos mecanismos moleculares que sustentam a doença, oferecendo novas perspectivas para a avaliação de fármacos já utilizados, como o alendronato de sódio, o raloxifeno e o ácido zoledrônico. Nesse contexto, este projeto busca explorar as principais vias metabólicas relacionadas à osteoporose e os alvos moleculares de seus tratamentos, utilizando bases de dados públicas e abordagens de modelagem em grafos para visualizar interações gênicas e farmacológicas. A motivação central é integrar dados ômicos e farmacológicos para evidenciar relações entre genes diferencialmente expressos, vias de sinalização e mecanismos de ação dos medicamentos, contribuindo para uma compreensão mais abrangente da doença e de suas terapias, com potenciais implicações para o desenho de novas estratégias terapêuticas de baixo custo e alta efetividade no sistema público de saúde.

# Slides

> [📄 PDF da apresentação](https://github.com/project-2025-data4health-group-7/Final-Project/blob/main/project-1/Entrega%201%20-%20Ciencia%20e%20visualiza%C3%A7%C3%A3o%20de%20dados%20em%20sa%C3%BAde.pdf)


# Fundamentação Teórica

A osteoporose é uma doença osteometabólica causada pela diminuição progressiva da densidade óssea e deterioração microarquitetural, tornando-os frágeis e porosos¹. Devido a fragilidade dos ossos, pacientes com essa doença possuem maior risco de fraturas, o que leva a dores e complicações a longo prazo diminuindo a qualidade de vida desses pacientes. Com o envelhecimento da população e o alto custo dos medicamentos no Brasil, a osteoporose torna-se um desafio para a saúde pública, tendo em vista a necessidade de medicamentos de alta efetividade e com baixo custo para a distribuição em larga escala pela rede pública de saúde².

Em condições normais, o osso é um órgão rígido e dinâmico que passa por um processo contínuo de remodelação envolvendo a "quebra" (reabsorção), feita por osteoclastos e construção de osso, feita por osteoblastos. Este processo ocorre em microescala por todo esqueleto durante toda a vida do ser humano. A osteoporose surge quando há um desequilíbrio nesse processo. Em pacientes com essa doença, o processo de reabsorção ocorre com maior frequência, de forma com que a síntese de novas camadas ósseas não conseguem acompanhar.

O aprofundamento sobre os mecanismos moleculares e genéticos, como por análise de associação genômica ampla (GWAS), podem contribuir para o entendimento da doença e para a busca de novas estratégias de intervenção no quadro clínico de pacientes. Uma vez que o mapa genético da doença se torna mais claro, é possível investigar como os tratamentos já existentes interagem com esses alvos. Nesse sentido, propõe-se a aplicação de uma metodologia de bioinformática, análoga à empregada por Yu et al. (2020), para avaliar os mecanismos de ação de medicamentos já estabelecidos e utilizados no tratamento da osteoporose: o alendronato de sódio, o raloxifeno e o ácido zoledrônico. 

# Perguntas de Pesquisa

1. Quais são as principais vias metabólicas relacionadas a osteoporose? 
 
2. Como os medicamentos mais indicados para osteoporose agem nas vias metabólicas dessa doença?

# Bases de Dados

> Os conjuntos de dados a serem utilizados nesse trabalho são advindos do GEO. Os códigos de acesso são: GSE7158, GSE56814 e GSE56815.

> Base de Dados | Endereço na Web | Resumo descritivo
> ----- | ----- | -----
> GEO | https://www.ncbi.nlm.nih.gov/geo/ | Repositório de dados genômicos do NCBI |
> String DB | https://string-db.org/ |  Banco de dados de interações proteína-proteína conhecidas e previstas |
> KEGG | https://www.genome.jp/kegg/ | Bancos de dados que serve para compreender funções e interações moleculares em sistemas biológicos |
> ChEMBL | https://www.ebi.ac.uk/chembl/ | Banco de dados de moléculas bioativas com propriedades semelhantes às de medicamentos |
> Open Targets Plataform | https://platform.opentargets.org/ | Banco de dados de alvos moleculares de medicamentos |
> GBQ Target identification | https://bioquimio.udla.edu.ec/tidentification01 | Banco de dados dos mecanismos de ação e efeitos colaterais de compostos químicos |
>
## Conjunto de dados

> Os conjuntos de dados a serem utilizados nesse trabalho são advindos do GEO. Os códigos de acesso são: GSE7158, GSE56814 e GSE56815.
> GEO accession | Endereço na Web | Resumo descritivo
> ----- | ----- | -----
> GSE7158 | https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE7158 | Estudo de expressão gênica em todo o genoma de monócitos circulantes em humanos com massa óssea extremamente alta vs. baixa |
> GSE56814 | https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE56814 | 	Estudo da expressão gênica de monócitos sanguíneos em mulheres na pré e pós-menopausa com baixa ou alta densidade mineral óssea |
> GSE56815 | https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE56815 | Estudo da expressão gênica de monócitos sanguíneos em mulheres na pré e pós-menopausa com baixa ou alta densidade mineral óssea |


# Modelo Lógico

<div align="center">
 <img width="1062" height="435" alt="image" src="https://github.com/user-attachments/assets/b5872d53-aace-4e61-9639-e5b369b3cc92" />
</div>


> O modelo lógico da base de grafos que será construída segue a no seguinte [link](https://docs.google.com/presentation/d/15b7ehktnPQX_y3pzP3UTcvcNo337se3j4HlWogn3MKo)

# Metodologia

> Para explorar as vias metabólicas da osteoporose e os alvos moleculares de seu tratamento realizaremos os seguinte passos: 

1. Identificar genes diferentemente expressos em osteoporose.

2. Classificar esses genes em perfis metabólicos do KEGG.

3. Selecionar vias metabólicas com potencial para os metabolismos envolvidos nessa doença.

4. Identificar genes com maior centralidade entre os genes envolvidos com a doença.

5. Identificar alvos moleculares das vias onde os medicamento utilizados atuam.

6. Comparar genes envolvidos nas vias destes tratamentos com os genes selecionados da doença.


# Ferramentas

> Utilizaremos as seguintes ferramentas:

 - Cytoscape: será utilizado para gerar grafos das vias metabolicas envolvidas com a osteorose e os alvos mocelulares dos medicamentos e realizar as associações.
 - KEGG: proverá as categorias semânticas das vias analisadas de modo a limitar as análises aos processos mais relacionados à doença.
 - Neo4J: permitirá realizarmos análises mais aprofundadas nas redes para obter padrões e compreender interações entre vias da doença e medicamentos.

# Referências Bibliográficas

> [1] MORAES, Luci Fabiane Scheffer et al. Expenditures on the treatment of osteoporosis in the elderly in Brazil (2008-2010): analysis of associated factors. Revista Brasileira de Epidemiologia, v. 17, p. 719-734, 2014.

> [2] YU, Tao et al. The shared KEGG pathways between icariin-targeted genes and osteoporosis. Aging (Albany NY), v. 12, n. 9, p. 8191, 2020.
