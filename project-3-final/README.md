
# Projeto `A Intersecção entre as Vias de sinalização envolvidas na Osteoporose e os Genes Alvos dos Medicamentos Raloxifeno, Ácido Zoledrônico e Alendronato de Sódio`
*2025.1 Ciência e Visualização de Dados em Saúde*

## Participantes
- Barbara da P. Perez Rodrigues - Instituto de Biologia
- Sophia de Alcantara Rodrigues - Faculdade de Ciências Médicas
- Pablo Alessandro Barbosa Viana - Instituto de Biologia
- Felipe Araújo de Lima - Instituto de Computação
- Thaynara Beatriz S. de Matos - Instituto de Computação



## Resumo
Este trabalho apresenta uma análise integrativa sobre a osteoporose, doença caracterizada pela redução da densidade e alterações na microarquitetura óssea, resultando em maior fragilidade dos ossos. Com alta prevalência mundial e impacto crescente no Brasil devido ao envelhecimento populacional, a osteoporose demanda abordagens terapêuticas eficazes e personalizadas.  

O estudo foca na intersecção entre as principais vias de sinalização envolvidas na osteoporose e os genes-alvos de três medicamentos amplamente utilizados no SUS (Sistema Único de Saúde): Raloxifeno, Ácido Zoledrônico e Alendronato de Sódio. Utilizando ferramentas aprendidas em sala de aula, foram analisados dados de expressão gênica de monócitos sanguíneos de mulheres, identificando genes diferencialmente expressos em tecidos de alta e baixa densidade óssea. A partir desses dados, foram mapeadas as vias de sinalização comuns e específicas moduladas por cada medicamento.  

Os resultados destacam que os três fármacos atuam em vias relacionadas a inflamação, remodelação óssea e sobrevivência celular, como “Cytokine Signaling”, “Interferon Alpha/Beta”, “Interferon Gamma”, “ESR Signaling” e “G Alpha Q Signaling”. O estudo evidencia mecanismos de ação distintos e complementares, reforçando a importância de abordagens personalizadas no tratamento de osteoporose.  

Além de contribuir para o entendimento dos efeitos moleculares dos medicamentos, o trabalho propõe uma metodologia comparativa e integrativa pouco explorada na literatura nacional, com potencial para orientar futuras pesquisas, validações experimentais e o desenvolvimento de estratégias terapêuticas mais eficazes.  



## Introdução
A osteoporose é uma doença esquelética sistêmica caracterizada pela redução da massa óssea e pela deterioração da microarquitetura do tecido ósseo, resultando em maior fragilidade e suscetibilidade a fraturas. Sua prevalência aumenta com a idade e é particularmente elevada entre mulheres pós-menopáusicas, tornando-se um problema crescente em países com rápido envelhecimento populacional (1). No Brasil, por exemplo, o número de indivíduos com 65 anos ou mais aumentou 57%, passando de 14,1 milhões em 2010 para 22,2 milhões em 2022 (2). As fraturas associadas à osteoporose acarretam declínios substanciais no estado funcional e na qualidade de vida, além de estarem relacionadas a significativa morbidade, mortalidade e custos médicos diretos (3). Em 2018, o ônus econômico da osteoporose em quatro países da América Latina, incluindo o Brasil, foi estimado em 1,17 bilhão de dólares. Ademais, a fratura inicial aumenta de forma acentuada o risco de fraturas subsequentes (3, 4).

O tecido ósseo passa por remodelação contínua por meio da atividade coordenada de osteoblastos, responsáveis pela formação óssea, e osteoclastos, responsáveis pela sua reabsorção. A osteoporose surge de um desequilíbrio entre esses dois processos, geralmente devido ao aumento da reabsorção mediada pelos osteoclastos. Os osteoclastos se originam de unidades formadoras de colônias de granulócitos-macrófagos (CFU-GM) na medula óssea, e sua diferenciação é estimulada por diversas citocinas pró-inflamatórias, cuja produção é normalmente regulada negativamente pelo estrogênio.

O estrogênio também modula a atividade do ligante do receptor ativador do fator nuclear κB (RANKL), um regulador essencial da osteoclastogênese. O RANKL, produzido pelos osteoblastos, liga-se ao receptor RANK nos precursores de osteoclastos, ativando vias de sinalização que promovem sua diferenciação, atividade e sobrevivência. O estrogênio aumenta a produção de osteoprotegerina (OPG), um receptor de sinal que neutraliza o RANKL e reduz a formação de osteoclastos. Além disso, o estrogênio estimula a apoptose dessas células por meio do sistema Fas/FasL.

A perda de estrogênio durante os períodos perimenopausal e pós-menopausal precoce acelera a perda óssea, especialmente nos primeiros cinco anos após a menopausa, estabilizando-se cerca de dez anos depois. A terapia estrogênica pós-menopausa pode atenuar esse processo ao suprimir a atividade osteoclástica (1, 4).

As terapias para osteoporose são classificadas em duas categorias principais: agentes antirreabsortivos — como hormônios, moduladores seletivos do receptor de estrogênio, bisfosfonatos e denosumabe — e agentes anabólicos, como teriparatida e abaloparatida (1, 4).

Os medicamentos antirreabsortivos inibem principalmente o recrutamento e a atividade dos osteoclastos, reduzindo as taxas de remodelação óssea e permitindo aumentos modestos na densidade mineral óssea (DMO) ao diminuir a formação de novas lacunas de reabsorção. Embora esses tratamentos não corrijam completamente o desequilíbrio da remodelação, a redução expressiva nas unidades de remodelação ativas diminui o impacto global desse desequilíbrio. A menor remodelação também leva a maior mineralização secundária, contribuindo para ganhos adicionais de DMO. Assim, a terapia antirreabsortiva preserva a massa e a estrutura óssea existentes enquanto promove uma mineralização mais uniforme (4).

Em contraste, agentes osteo-anabólicos estimulam a formação óssea ao aumentar o número e a atividade dos osteoblastos, levando a um rápido aumento da formação, seguido por um incremento mais lento da reabsorção (5).

No Brasil, o Sistema Único de Saúde (SUS) disponibiliza gratuitamente uma ampla gama de tratamentos para osteoporose. Esses medicamentos são oferecidos por meio do Componente Básico da Assistência Farmacêutica — distribuído em farmácias da atenção primária — e do Componente Especializado, que inclui opções terapêuticas de maior custo. Entre os tratamentos disponíveis estão bisfosfonatos (como alendronato de sódio, risedronato de sódio, pamidronato dissódico e ácido zoledrônico), carbonato de cálcio, calcitriol, vitamina D (colecalciferol), raloxifeno, terapia hormonal, calcitonina, denosumabe e teriparatida. A escolha terapêutica é individualizada, considerando fatores como idade, sexo, gravidade da doença, histórico de fraturas, comorbidades e preferências do paciente (6).

Embora medicamentos como raloxifeno, ácido zoledrônico e alendronato sejam amplamente utilizados no Brasil para prevenir fraturas e retardar a progressão da osteoporose, seus mecanismos moleculares completos — especialmente os que envolvem vias de sinalização cruciais para a patogênese da doença — ainda não foram totalmente elucidados. Essa lacuna levanta questões relevantes: quais alvos e vias moleculares específicas são modulados por cada um desses fármacos? Esses medicamentos compartilham mecanismos de ação ou atuam por rotas distintas? E de que forma esses mecanismos podem influenciar a otimização e a personalização do tratamento da osteoporose? Esclarecer essas questões é fundamental para aprimorar a precisão terapêutica e melhorar os desfechos clínicos.

Diante desse cenário, o presente estudo torna-se particularmente relevante. Ao integrar análises computacionais, identifica mecanismos moleculares compartilhados entre esses fármacos e esclarece como cada um interage com alvos e vias de sinalização específicas. Esses conhecimentos podem orientar combinações terapêuticas mais racionais, minimizar efeitos sobrepostos e revelar interações sinérgicas capazes de aumentar a eficácia com doses menores. Em última instância, ao traduzir dados genômicos e proteômicos em insights clinicamente significativos, este estudo fortalece a interface entre biologia molecular e prática médica, oferecendo suporte mais robusto e baseado em evidências para a tomada de decisões terapêuticas.



## Metodologia (B)
A metodologia deste trabalho foi planejada visando atingir o objetivo de identificação dos genes que participam da patologia da osteoporose e de que forma os medicamentos atuam visando atingi-los e, dessa forma, mitigar a doença. Para isso buscou-se na literatura trabalhos que se alinhassem com a proposta do projeto para a identificação das ferramentas mais utilizadas e procedimentos experimentais validados para aplicação no trabalho.

### 2.1 Bases de dados e Evolução
Para o desenvolvimento do trabalho foram utilizadas uma série de bases de dados para obtenção das informações relacionadas à ação dos medicamentos, as formas de interação entre os genes, tanto os diferencialmente expressos, quanto os alvos de fármacos e também para obter as vias de sinalização na qual esses genes estão presentes.

Primeiramente, o conjunto de dados a respeito da expressão gênica comparativa entre pacientes portadores da osteoporose e os grupos controle sem a doença foram obtidos do “Gene Expression Omnibus” (GEO), banco de dados público mantido pelo NCBI (National Center for Biotechnology Information). Seus códigos de acesso são: GSE7158, GSE56814 e GSE56815, um resumo descritivo e o endereço de acesso a eles pode ser visto abaixo.

| GEO accession | Endereço na Web | Resumo descritivo |
|---------------|-----------------|--------------------|
| GSE7158 | https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE7158 | Estudo de expressão gênica em todo o genoma de monócitos circulantes em humanos com massa óssea extremamente alta vs. baixa |
| GSE56814 | https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE56814 | Estudo da expressão gênica de monócitos sanguíneos em mulheres na pré e pós-menopausa com baixa ou alta densidade mineral óssea |
| GSE56815 | https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE56815 | Estudo da expressão gênica de monócitos sanguíneos em mulheres na pré e pós-menopausa com baixa ou alta densidade mineral óssea |

Todos os experimentos utilizados para obtenção destes dados foram feitos a partir de monócitos circulantes na corrente sanguínea, é válido reiterar que estas células são aquelas que se diferenciam em osteoclastos, que promovem a reabsorção da matriz óssea. No entanto, o grupo de pacientes alvo para cada um dos estudos foi diferente. O estudo registrado pelo GSE7158 contém dados de homens e mulheres com massa óssea extremamente alta e baixa. Já o GSE56814 e o GSE56815 são de mulheres pré e pós-menopausa com baixa ou alta densidade mineral óssea.

Visando identificar quais proteínas são as alvo dos medicamentos, utilizamos o software Target identification v1 (Bio-Chemoinformatics Group - BCG), o qual utiliza em seu modelo informações advindas do banco de dados ChEMBL o qual contém dados de moléculas bioativas com propriedades semelhantes às de medicamentos e os genes com o qual esses fármacos interagem.

Já para a obtenção das interações entre os genes foi utilizado o banco de dados de interação proteína-proteína, STRING-db. Por fim, para identificar as vias de sinalização em que os genes participavam utilizamos o David Bioinformatics selecionando o agrupamento funcional do Reactome, que contém informações sobre vias biológicas e reações moleculares.

| Base de Dados | Endereço na Web | Resumo descritivo |
|---------------|-----------------|--------------------|
| GEO | https://www.ncbi.nlm.nih.gov/geo/ | Repositório de dados genômicos do NCBI |
| ChEMBL | https://www.ebi.ac.uk/chembl/ | Banco de dados de moléculas bioativas com propriedades semelhantes às de medicamentos |
| STRING-db | https://string-db.org/ | Banco de dados de interações proteína-proteína conhecidas e previstas |
| Reactome | https://reactome.org/ | Banco de dados de reações biológicas e vias moleculares |

---

### 2.2 Modelo Lógico
Para construir nossa rede, primeiro identificamos os tipos de entidades e as relações entre elas que desejamos visualizar. As amostras, doença, drogas, genes e vias de sinalização relacionam-se conforme o modelo da figura 1.


![Figura 01. Modelo lógico das redes](data/primeira_foto.png)

![Figura 02. Modelo da representação dos genes que são alvos dos medicamentos e que compõem as vias de sinalização envolvidas com genes diferencialmente expressos. Onde, o medicamento está representado por um losango (roxo), vias de sinalização como flechas para baixo (azul), genes diferentemente expressos positivamente como triângulos para cima (verde) e negativamente como triângulos para baixo (vermelho) e demais genes como elipses (bege)](data/segunda_foto.png)

---

### 2.3 Integração entre Bases
O trabalho envolveu uma abordagem integrativa e multidisciplinar, combinando diferentes ferramentas e etapas para investigar os mecanismos moleculares da osteoporose e a atuação dos medicamentos.  
Para correlacionar resultados encontrados nas diferentes bases utilizamos o EntrezID. A partir da análise de expressão diferencial coletamos o EntrezID dos genes diferencialmente expressos nos diferentes conjuntos de dados selecionados. Estes genes foram submetidos ao David onde coletamos as informações das vias de sinalização a que pertencem no Reactome.  
Paralelamente, foram identificados os genes-alvo de cada medicamento, a partir do banco de dados farmacogenéticos do CHEMBL (usando a ferramenta Target Identification v1 do BCG). Também coletamos os EntrezID desses genes e os submetemos ao David, descobrindo as vias de sinalização a que pertencem no Reactome.  
Seguimos apenas com as vias em que foram encontrados genes diferencialmente expressos e que possuíam algum gene alvo dos medicamentos. No Reactome coletamos a lista completa de genes de cada uma dessas vias e agrupamos com os genes alvos dos medicamentos e genes diferencialmente expressos. Por fim, submetemos essa lista ao STRING-db para obter o grafo de interação proteína-proteína.

---

### 2.4 Análises Realizadas
Integração dos resultados  
As vias de sinalização comuns e específicas moduladas por Alendronato, Raloxifeno e Ácido Zoledrônico foram comparadas, destacando mecanismos de ação distintos e complementares. O estudo evidenciou a atuação dos medicamentos em vias relacionadas a inflamação, remodelação óssea e sobrevivência celular.

Análise integrada do dataset GSE56815  
A fim de comparar de modo aprofundado a correlação entre genes diferencialmente expressos na doença e todos os alvos de medicamentos de modo integrado, selecionamos o dataset maior e mais completo, o GSE56815, realizando algumas análises computacionais adicionais.  
Primeiramente, os genes do dataset foram selecionados e inseridos no STRING-db, gerando uma rede de interações físicas (confidence > 0.7, fontes experimentais e bancos de dados). Os genes relacionados aos 3 medicamentos foram então adicionados à rede, permitindo visualizar sobreposições e conexões entre os alvos terapêuticos e os genes associados à doença.  
Utilizando as bibliotecas pandas, networkx e pyvis, foram realizadas análises de centralidade, detecção de comunidades e avaliação de proximidade entre genes expressos e genes-alvo de medicamentos. Foram criadas visualizações interativas, diferenciando os grupos por cores e formatos, facilitando a interpretação dos resultados e a identificação de genes-chave e potenciais pontos de intervenção.  
Tal análise evidenciou como o Raloxifeno tem uma atuação diferente dos outros dois medicamentos, além de nenhum dos medicamentos estarem envolvidos com os genes diferencialmente expressos da doença. No entanto, o que foi notado é que os medicamentos (no geral), estão na vizinhança dos genes diferencialmente-expressos, atuando de forma indireta.


---

### 2.5 Evolução do Projeto
Todo o trabalho explorou algumas áreas de conhecimento no qual os alunos não tinham tido tanto contato até então. Assim, todo o desenvolvimento da metodologia foi um grande desafio o qual demandou muita leitura e consulta da literatura.  
No início do projeto, foram seguidas as etapas tradicionais de análise de expressão gênica diferencial conforme apresentadas em sala de aula pelos professores. Paralelamente, também foram obtidos os genes-alvo dos medicamentos utilizados no tratamento da doença. Com ambos os conjuntos de dados disponíveis, surgiu o desafio de integrá-los de maneira a gerar uma interpretação mais ampla sobre a relação entre a doença e os fármacos. A primeira estratégia foi cruzar as informações, buscando identificar genes que fossem ao mesmo tempo diferencialmente expressos na doença e também alvos diretos dos medicamentos. A partir dessa interseção, os dados seriam enviados para o DAVID com o objetivo de realizar enriquecimento funcional e identificar vias de sinalização relacionadas.  
No entanto, essa abordagem mostrou-se limitada, pois resultou na identificação de poucos genes em comum. Além disso, ela desconsiderava um ponto importante: mesmo que um medicamento não tenha como alvo direto uma proteína diferencialmente expressa, ele pode atuar sobre outra proteína que interage com ela e, indiretamente, afetar o processo biológico da doença. Essa percepção motivou a reavaliação da estratégia inicial, indicando a necessidade de expandir as análises para considerar redes de interação e relações funcionais mais amplas, permitindo uma visão mais realista e abrangente dos mecanismos envolvidos.  
Assim, ao final, decidiu-se utilizar como entrada no DAVID todos os genes diferencialmente expressos e todos os alvos dos medicamentos de forma conjunta. Dessa maneira, foi possível identificar vias de sinalização nas quais genes de ambos os conjuntos participavam, com base no output fornecido pelo Reactome. A partir desses resultados, foram selecionadas as vias mais relevantes, definidas como aquelas que apareciam nas duas formas de análise: tanto pela busca baseada nos genes diferencialmente expressos quanto na busca baseada nos alvos dos medicamentos.  
Em seguida, foram extraídos os genes participantes dessas vias de sinalização e, com essas informações, identificaram-se os alvos dos medicamentos dentro desse contexto. Essa integração permitiu uma primeira interpretação conjunta dos dados, evidenciando relações funcionais e interações biológicas que não seriam observadas ao analisar os conjuntos separadamente. Por fim, a visualização em rede no Cytoscape possibilitou uma compreensão mais clara e integrada dessas interações.


## Ferramentas
A metodologia proposta exigiu o uso de múltiplas ferramentas durante as etapas. Estão listadas a seguir as plataformas e ferramentas essenciais para a execução da metodologia proposta:

- **Orange**: Utilizado na preparação dos dados advindos do GEO. Essa ferramenta auxiliou no cálculo do logFC e do p-value da expressão diferencial.

- **Ferramenta de identificação de targets do grupo Bio-Chemoinformatics**: Essa ferramenta foi utilizada como fonte dos genes alvos de cada medicamento estudado. É importante destacar que, no artigo de referência [7], os alvos foram obtidos através do database STITCH (Search Tool for Interactions of Chemicals). No entanto, optou-se por não utilizar o STITCH neste trabalho devido à sua indisponibilidade durante o período de execução do projeto.

- **David Bioinformatics**: Necessário para encontrar as principais vias nas quais os genes estão envolvidos.

- **Reactome**: Esse banco de dados foi utilizado como fonte para alcançar os genes presentes em cada uma das vias de sinalização de interesse identificadas.

- **Python**: Foram construídos scripts em Python para realizar tarefas de manipulação de dados como o mapeamento e conversão entre tipos de IDs das proteínas e genes, como de uniprot para entrez ID, permitindo que as buscas nas diferentes plataformas e ferramentas fossem realizadas com sucesso. A intersecção entre os conjuntos das principais vias dos genes alvo e dos genes diferencialmente expressos também foi feita via Python. Por fim, a organização dos arquivos de entrada para a construção das redes foi realizada da mesma maneira.

- **Cytoscape**: Utilizado na visualização das redes e estudos sobre comunidades.



## Discussão
A análise desenvolvida neste estudo reforça que a osteoporose é uma condição multifatorial complexa, caracterizada pela desregulação simultânea de vias de sinalização envolvidas na inflamação, na remodelação óssea e na sobrevivência celular, conforme amplamente descrito em revisões recentes sobre os determinantes genéticos e moleculares da doença (16, 17). Em condições fisiológicas, a integridade do tecido ósseo depende de um equilíbrio dinâmico entre formação e reabsorção, sustentado pela interação coordenada entre osteoblastos, osteócitos e osteoclastos (1, 18). A ativação aberrante de vias reguladas por citocinas, interferons, receptores hormonais e proteínas G promove um desequilíbrio profundo dessa homeostase, culminando em perda progressiva de densidade mineral e fragilidade óssea (7, 13, 20).

A integração dos dados demonstra que os três medicamentos analisados — alendronato, ácido zoledrônico e raloxifeno — apresentam mecanismos de ação distintos, mas convergem para vias centrais na regulação da osteoclastogênese e da remodelação óssea, o que é consistente com a natureza sistêmica da osteoporose, em que múltiplas camadas bioquímicas e celulares interagem de maneira interdependente (1, 3, 5). Um achado particularmente relevante é que esses fármacos não atuam majoritariamente sobre os genes que se encontram desregulados na doença, mas sim sobre genes que participam das mesmas vias de sinalização alteradas, fenômeno também observado em análises de vias compartilhadas entre alvos farmacológicos e a fisiopatologia óssea (7). Isso indica que seu efeito terapêutico ocorre por meio da modulação indireta dessas vias, ao interferirem em pontos estratégicos de controle funcional dentro das redes, mesmo quando seus alvos diretos não correspondem aos genes diferencialmente expressos — observação coerente com a literatura molecular e farmacológica sobre remodelação óssea (13, 20).

Os bisfosfonatos alendronato e ácido zoledrônico atuam primordialmente por meio da inibição de enzimas metabólicas essenciais à sobrevivência dos osteoclastos, especialmente FDPS e GGPS1, conforme amplamente estabelecido em estudos sobre o mecanismo de ação dessa classe de fármacos (8, 9). A supressão dessas enzimas bloqueia a síntese de farnesil pirofosfato e geranilgeranil pirofosfato, compostos indispensáveis para a prenilação de proteínas GTPases envolvidas na adesão, motilidade e atividade reabsortiva dos osteoclastos (8). Essa interrupção leva ao colapso da organização citoesquelética e funcional dessas células, culminando em apoptose e consequente redução da reabsorção óssea, efeito também corroborado por evidências que demonstram a participação de espécies reativas de oxigênio nesse processo (12). Além da interferência metabólica, os bisfosfonatos também modulam vias intracelulares amplamente implicadas na diferenciação e ativação osteoclástica, como JAK–STAT, MAPK e PI3K–AKT, mecanismos discutidos em estudos pré-clínicos e clínicos (10, 11). Entre esses fármacos, o ácido zoledrônico destaca-se pela maior afinidade por FDPS e pelos efeitos anti-reabsortivos de longa duração, como demonstrado nos principais ensaios clínicos pivôs (11, 12).

O raloxifeno apresenta um mecanismo de ação complementar, baseado na modulação seletiva dos receptores de estrogênio ESR1 e ESR2, conforme amplamente detalhado na literatura sobre SERMs aplicados à osteoporose (14, 15). Em condições normais, o estrogênio limita a expressão de citocinas pró-osteoclásticas e regula o eixo RANK/RANKL/OPG, indispensável para controlar a diferenciação e ativação dos osteoclastos (3, 20). A queda estrogênica pós-menopausa desestabiliza esse eixo, favorecendo a reabsorção óssea (3). Ao ativar seletivamente ESR1 e ESR2 no tecido ósseo, o raloxifeno restaura parte desse controle, reduzindo a formação de novos osteoclastos e diminuindo a atividade das células maduras (14, 15). A modulação de vias associadas a citocinas e interferons — incluindo genes como CXCL10, CXCL11 e C3 — confere ao raloxifeno efeitos adicionais sobre a inflamação, reforçando dados que associam quimiocinas e vias inflamatórias ao risco aumentado de perda óssea (19, 20).

Embora seus mecanismos moleculares sejam distintos, os três medicamentos convergem para vias centrais da remodelação óssea. Todos interferem, direta ou indiretamente, na via RANK/RANKL/OPG, eixo-chave da osteoclastogênese (1, 3, 5), além de modular vias inflamatórias como Cytokine Signaling e Interferon Alpha/Beta (13, 20). Genes relacionados à sobrevivência e ativação celular, incluindo MAPK1, MAPK3, AKT2 e JAK1, emergem como pontos comuns de modulação entre os tratamentos, sugerindo que esses elementos podem representar alvos estratégicos para terapias mais precisas e biomarcadores de resposta terapêutica (7, 13, 16).

Esses achados evidenciam que a efetividade no tratamento da osteoporose depende da intervenção coordenada em múltiplos níveis regulatórios — metabólicos, hormonais e imunológicos (1, 3, 5) — e reforçam a importância de abordagens terapêuticas individualizadas, especialmente diante do impacto crescente da doença em populações envelhecidas, como observado no contexto brasileiro e latino-americano (2, 4, 6). A integração entre dados moleculares e clínicos destaca-se como uma ferramenta útil para compreender como diferentes fármacos impactam a remodelação óssea em diferentes escalas biológicas, contribuindo para otimizar a eficácia terapêutica e reduzir efeitos adversos (5, 13).




## Conclusão
Os achados deste estudo evidenciam que, embora os fármacos amplamente utilizados no tratamento da osteoporose — alendronato, ácido zoledrônico e raloxifeno — apresentem mecanismos de ação distintos, eles convergem para vias biológicas centrais envolvidas na regulação da remodelação óssea. A análise integrada revelou que esses medicamentos não atuam predominantemente sobre genes diferencialmente expressos na doença, mas modulam de forma indireta vias de sinalização críticas, reforçando a complexidade da interação entre farmacologia e fisiopatologia óssea.

Esses resultados sugerem que intervenções terapêuticas eficazes podem atuar estrategicamente em nodos funcionais paralelos dentro das mesmas redes moleculares alteradas, restaurando seu equilíbrio global mesmo sem direcionamento direto aos genes desregulados. Essa compreensão aprofunda a visão sistêmica da osteoporose e amplia a perspectiva sobre o funcionamento dos tratamentos atualmente disponíveis.

Além disso, as perspectivas delineadas no presente trabalho apontam caminhos promissores para validações experimentais, integração com dados ômicos e exploração de potenciais biomarcadores, contribuindo para o avanço do entendimento mecanístico e para o desenvolvimento de estratégias terapêuticas mais precisas e personalizadas no manejo da osteoporose.



## Trabalhos Futuros
Como continuidade natural deste estudo, futuros trabalhos deverão aprofundar a compreensão das interações entre medicamentos anti-osteoporóticos e suas vias de sinalização associadas. Inicialmente, serão realizadas simulações de dinâmica molecular, com o objetivo de avaliar a afinidade, estabilidade conformacional e energia de ligação entre os fármacos estudados e os principais alvos proteicos identificados. Essa abordagem permitirá validar, em nível estrutural, a plausibilidade das interações previstas in silico e identificar resíduos críticos da interface fármaco–receptor.

Também, será essencial correlacionar os alvos moleculares mapeados neste estudo com dados de expressão gênica e proteica obtidos diretamente de tecidos ósseos humanos, tanto sadios quanto acometidos por osteoporose. Essa integração permitirá determinar se os genes e proteínas modulados pelos medicamentos apresentam relevância fisiológica no microambiente ósseo, fortalecendo a validade biológica dos achados. Em seguida, pretende-se validar experimentalmente os principais alvos e vias sinalizadas, utilizando modelos celulares e, quando possível, análises ex vivo. Ensaios funcionais envolvendo osteoblastos, osteoclastos e células do estroma ósseo poderão confirmar os efeitos preditos sobre diferenciação, atividade enzimática e remodelação óssea.

Por fim, será conduzida uma análise translacional para identificar biomarcadores de resposta terapêutica e avaliar o potencial dos alvos identificados para apoiar decisões clínicas personalizadas. Esses resultados poderão indicar novos usos para medicamentos já disponíveis, propor combinações terapêuticas mais eficientes e revelar vias pouco exploradas que merecem investigação em estudos pré-clínicos e clínicos.



## Referências Bibliográficas
1. Compston JE, McClung MR, Leslie WD. Osteoporosis. Lancet. 2019; 393(10169): 364-76.  
2. Kirby T. Brazil facing ageing population challenges. Lancet. 2023;402(10415):1821.  
3. Muñoz BA, Robinson K, Shibli-Rahhal A. Bone health and osteoporosis prevention and treatment. Clin Obstet Gynecol. 2020;63(4):770-7.  
4. Aziziyeh R, Amin M, Habib M, Garcia Perlaza J, Szafranski K, McTavish RK, et al. The burden of osteoporosis in four Latin American countries: Brazil, Mexico, Colombia, and Argentina. J Med Econ. 2019;22(7):638-44.  
5. Bandeira L, Lewiecki EM. Anabolic therapy for osteoporosis: update on efficacy and safety. Arch Endocrinol Metab. 2022;66(5):707-16.  
6. Viva o SUS. Osteoporosis: prevention and treatment by the SUS [Internet]. 2025 [cited 2025 Nov 14]. Available from: https://vivaosus.com/osteoporose  
7. Yu T. The shared KEGG pathways between icariin-targeted genes and osteoporosis. Aging (Albany NY). 2020;12(9):8191-201.  
8. Reszka, A.A., Rodan, G.A. Bisphosphonate mechanism of action. Curr Rheumatol Rep 5, 65–74 (2003).  
9. Agabiti SS, Liang Y, Wiemer AJ. Molecular mechanisms linking geranylgeranyl diphosphate synthase to cell survival and proliferation. Mol Membr Biol. 2016 Mar;33(1-2):1-11.  
10. Ma X, Xu Z, Ding S, Yi G, Wang Q. Alendronate promotes osteoblast differentiation and bone formation in ovariectomy-induced osteoporosis through interferon-β/signal transducer and activator of transcription 1 pathway. Exp Ther Med. 2018 Jan;15(1):182-190.  
11. Black DM, Delmas PD, Eastell R, et tal. HORIZON Pivotal Fracture Trial. Once-yearly zoledronic acid for treatment of postmenopausal osteoporosis. N Engl J Med. 2007 May 3;356(18):1809-22.  
12. Tai TW, Chen CY, Su FC, Tu YK, Tsai TT, Lin CF, Jou IM. Reactive oxygen species are required for zoledronic acid-induced apoptosis in osteoclast precursors and mature osteoclast-like cells. Sci Rep. 2017 Mar 10;7:44245.  
13. Dhillon S. Zoledronic Acid (Reclast®, Aclasta®): A Review in Osteoporosis. Drugs. 2016 Nov;76(17):1683-1697.  
14. Clemett D, Spencer CM. Raloxifene: a review of its use in postmenopausal osteoporosis. Drugs. 2000 Aug;60(2):379-411.  
15. D'Amelio P, Isaia GC. The use of raloxifene in osteoporosis treatment. Expert Opin Pharmacother. 2013 May;14(7):949-56.  
16. Lu HF, Chou PH, Lin GH, Chou WH, Wang ST, Adikusuma W, Mugiyanto E, Hung KS, Chang WC. Pharmacogenomics Study for Raloxifene in Postmenopausal Female with Osteoporosis. Dis Markers. 2020 Aug 31;2020:8855423.  
17. Yang TL, Shen H, Liu A, Dong SS, Zhang L, Deng FY, Zhao Q, Deng HW. A road map for understanding molecular and genetic determinants of osteoporosis. Nat Rev Endocrinol. 2020 Feb;16(2):91-103.  
18. Munro Peacock, Charles H. Turner, Michael J. Econs, Tatiana Foroud, Genetics of Osteoporosis, Endocrine Reviews, Volume 23, Issue 3, 1 June 2002, Pages 303–326.  
19. Long F Building strong bones: molecular regulation of the osteoblast lineage. Nat. Rev. Mol. Cell Biol 13, 27–38.  
20. Elahmer NR, Wong SK, Mohamed N, Alias E, Chin KY, Muhammad N. Mechanistic Insights and Therapeutic Strategies in Osteoporosis: A Comprehensive Review. Biomedicines. 2024 Jul 23;12(8):1635.  
21. Wojdasiewicz P, Turczyn P, Dobies-Krzesniak B, Frasunska J, Tarnacka B. Role of CX3CL1/CX3CR1 Signaling Axis Activity in Osteoporosis. Mediators Inflamm. 2019 Nov 12;2019:7570452.  
22. De Martinis M, Sirufo MM, Suppa M, Ginaldi L. IL-33/IL-31 Axis in Osteoporosis. Int J Mol Sci. 2020 Feb 13;21(4):1239.  

