# pratica_House_Prices

## **PRIMEIRA ENTREGA DO PROJETO FINAL**

**Formato:** Link para o repositório de Github ou documento de Jupyter.
**Sugestão:** Se optarem por realizar o projeto em equipe, apenas um membro da equipe deverá entregar o desafio pela plataforma.

<hr>

**Objetivos Gerais:**

1. Entender o problema de negócio e identificar os elementos a serem considerados para o planejamento de um Modelo de Data Science.
2. Descrever os dados do problema e as relações entre dados através da Análise Exploratória de Dados.
3. Construir uma apresentação executiva mostrando os resultados obtidos.

**Objetivos Específicos:**

1. Desenvolver as instâncias de Data Acquisition e Data Wrangling em seu trabalho final.
2. Conseguir uma articulação em equipe e uma divisão de tarefas adequadas aos objetivos.
3. Realizar Filtragem.
4. Descrever o que significa cada variável, como se comporta.
5. Especificar as distribuições e relações (gêneros, sexo, idade, tributação, tipo de empresa).

**Deverá entregar:**

* Apresentação da empresa ou problema específico.
* Perguntas e objetivos da pesquisa.
* Configuração da equipe de trabalho.
* Indicação da fonte do dataset e os critérios de seleção (Data Acquisition).
* Geração do primeiro Data Wrangling e EDA, apontado seus dados (insights) univariados, bivariados e multivariados.
* Análise de Componentes Principais.
* Contar a história de seus dados.
* Filtros aplicados aos dados. Distribuição. Dataset final para analisar.
* Analisar objetivos ou objetivo para esses dados.

<hr>

## **MSSubClass**

A coluna **`MSSubClass`** no dataset refere-se à  **classe do tipo de construção residencial** . Cada valor em **`MSSubClass`** representa um código numérico que identifica o tipo de construção do imóvel, com base em características como o estilo, o tipo de construção, e a idade.

Aqui estão alguns exemplos de códigos **`MSSubClass`** e seus significados:

* **20** : 1-Story (Andar único) de 1946 ou posterior
* **30** : 1-Story (Andar único) de 1945 ou anterior
* **40** : 1-Story with Finished Attic (Andar único com sótão acabado)
* **45** : 1-1/2 Story - Unfinished (Andar e meio - inacabado)
* **50** : 1-1/2 Story - Finished (Andar e meio - acabado)
* **60** : 2-Story (Dois andares) de 1946 ou posterior
* **70** : 2-Story de 1945 ou anterior
* **75** : 2-1/2 Story (Dois andares e meio)
* **80** : Split or Multi-Level (Nível dividido ou multi-nível)
* **85** : Split Foyer (Nível dividido com saguão)
* **90** : Duplex - All Styles and Ages (Duplex - Todos os estilos e idades)
* **120** : 1-Story PUD (Planned Unit Development - Desenvolvimento de Unidade Planejada) - Andar único
* **150** : 1-1/2 Story PUD
* **160** : 2-Story PUD
* **190** : 2 Family Conversion - todas as idades (Conversão de família dupla)

Essa coluna ajuda a classificar os imóveis com base no tipo de construção, o que pode ser um fator importante na determinação do valor do imóvel.

## **LotFrontage**

A coluna **`LotFrontage`** no dataset refere-se à **largura da frente do terreno** do imóvel, medida em  **pés lineares** . Ela representa a extensão da parte da propriedade que faz frente para a rua ou estrada.

Basicamente, o **`LotFrontage`** indica o tamanho da fachada do lote, o que pode influenciar no valor do imóvel, já que lotes com frentes maiores costumam ser mais valiosos, especialmente em áreas urbanas, onde o espaço é mais restrito.

Exemplo:

* Se **`LotFrontage`** for 60, isso significa que a frente do terreno tem 60 pés (cerca de 18,3 metros).

## **LotArea**

A coluna **`LotArea`** no dataset refere-se ao **tamanho total do lote do imóvel** em  **pés quadrados** .

Ela representa a área total do terreno em que a propriedade está localizada, o que inclui todas as suas dimensões (não apenas a frente, mas também a profundidade). Esse valor é importante porque o tamanho do lote pode influenciar diretamente o preço de venda do imóvel, sendo lotes maiores geralmente mais valiosos.

Exemplo:

* Se **`LotArea`** for 10.000, isso significa que o terreno tem 10.000 pés quadrados (cerca de 929 metros quadrados).

## **OverallQual**

A coluna **`OverallQual`** no dataset refere-se à  **qualidade geral dos materiais e acabamento da casa** . Esse valor é uma avaliação subjetiva, em uma escala de  **1 a 10** , que indica a qualidade global da construção, incluindo o tipo de material utilizado e o nível de acabamento.

Aqui está a escala com seu significado:

* **1** : Muito Ruim
* **2** : Ruim
* **3** : Abaixo da Média
* **4** : Mediana/Justa
* **5** : Média
* **6** : Acima da Média
* **7** : Boa
* **8** : Muito Boa
* **9** : Excelente
* **10** : Luxuosa

Esse atributo é importante na determinação do preço do imóvel, já que uma qualidade de construção mais alta normalmente resulta em um valor de venda mais alto.

## **OverallCond**

A coluna **`OverallCond`** no dataset refere-se à  **condição geral da casa** , ou seja, o estado de conservação do imóvel como um todo. Assim como a  **`OverallQual`** , é uma avaliação subjetiva, mas foca na condição do imóvel em termos de desgaste e manutenção, em vez de qualidade dos materiais.

A escala também vai de  **1 a 10** , com os seguintes significados:

* **1** : Muito Ruim
* **2** : Ruim
* **3** : Abaixo da Média
* **4** : Mediana/Justa
* **5** : Média
* **6** : Acima da Média
* **7** : Boa
* **8** : Muito Boa
* **9** : Excelente
* **10** : Impecável/Perfeita

Essa coluna ajuda a entender o estado de conservação da propriedade, influenciando o valor do imóvel, já que casas em melhores condições tendem a ter preços mais altos.

## **YearBuilt**

A coluna **`YearBuilt`** no dataset refere-se ao  **ano em que a casa foi originalmente construída** . Esse valor indica a data de construção inicial do imóvel, sem considerar possíveis reformas ou modificações feitas posteriormente.

O **ano de construção** é um fator relevante para avaliar a idade da propriedade e pode impactar o valor de venda. Casas mais antigas podem ter um valor menor, dependendo de seu estado de conservação e estilo arquitetônico, enquanto casas mais novas podem ser mais valorizadas, especialmente se forem construídas com materiais modernos e técnicas de construção atualizadas.

## **YearRemodAdd**

A coluna **`YearRemodAdd`** no dataset refere-se ao  **ano em que a casa foi reformada ou ampliada** . Se a casa nunca passou por uma reforma, o valor desta coluna será o mesmo da coluna **`YearBuilt`** (ano de construção original). Essa variável indica quando a casa recebeu uma renovação significativa, como uma atualização estrutural, de materiais, ou de design.

Este campo é importante porque uma reforma pode aumentar o valor do imóvel, mesmo que ele seja antigo. Imóveis reformados tendem a ser mais atraentes para compradores, pois podem oferecer melhorias que atendem a padrões mais modernos.

## **MasVnrArea**

A coluna **`MasVnrArea`** no dataset refere-se à **área da alvenaria decorativa externa** (em inglês,  *masonry veneer area* ), medida em  **pés quadrados** . Ela indica o tamanho da área externa da casa coberta por uma camada de alvenaria, que pode ser composta por tijolos, pedras ou outros materiais de revestimento.

Esse tipo de alvenaria é frequentemente usado para fins estéticos e pode aumentar o valor da propriedade, já que agrega beleza e durabilidade à fachada da casa.

Exemplo:

* Se **`MasVnrArea`** for 200, significa que a área da alvenaria decorativa na fachada da casa tem 200 pés quadrados (aproximadamente 18,6 metros quadrados).

## **BsmtFinSF1**

A coluna **`BsmtFinSF1`** no dataset refere-se à **área em pés quadrados** do **porão finalizado de tipo 1** ( *Type 1 Finished Square Feet* ). Esta coluna indica o tamanho da área do porão que foi finalizada com materiais de qualidade superior, como pisos, paredes e tetos acabados, tornando essa área utilizável como um espaço adicional na casa, como um quarto, sala de estar ou escritório.

O **"Tipo 1"** geralmente se refere à área do porão que foi finalizada de maneira primária ou mais significativa, diferenciando-a de outras partes do porão que podem ter um nível inferior de acabamento ou serem deixadas inacabadas.

Exemplo:

* Se **`BsmtFinSF1`** for 800, significa que 800 pés quadrados (cerca de 74,3 metros quadrados) do porão foram finalizados com acabamentos de qualidade.

## **BsmtFinSF2**

A coluna **`BsmtFinSF2`** no dataset refere-se à **área em pés quadrados** do **porão finalizado de tipo 2** ( *Type 2 Finished Square Feet* ). Assim como  **`BsmtFinSF1`** , essa coluna indica o tamanho da área do porão que foi finalizada, mas com materiais ou acabamentos de qualidade inferior em comparação ao tipo 1.

O **"Tipo 2"** pode se referir a uma área do porão que foi finalizada, mas de forma menos elaborada, como um espaço que não é utilizado para finalidades residenciais, mas que ainda possui um certo nível de acabamento.

Exemplo:

* Se **`BsmtFinSF2`** for 400, isso significa que 400 pés quadrados (cerca de 37,2 metros quadrados) do porão foram finalizados com acabamentos de qualidade inferior.

## **BsmtUnfSF**

A coluna **`BsmtUnfSF`** no dataset refere-se à **área em pés quadrados** do **porão não finalizado** ( *Unfinished Square Feet* ). Essa coluna indica o tamanho da área do porão que ainda não foi finalizada, ou seja, não possui acabamentos como piso, paredes ou tetos, e não é considerada utilizável como espaço habitável.

Essas áreas podem ser utilizadas para armazenamento ou outras funções, mas não são formalmente reconhecidas como espaços de vida devido à falta de acabamentos adequados.

Exemplo:

* Se **`BsmtUnfSF`** for 600, isso significa que 600 pés quadrados (cerca de 55,7 metros quadrados) do porão permanecem não acabados.

## **TotalBsmtSF**

A coluna **`TotalBsmtSF`** no dataset refere-se à **área total do porão** (em pés quadrados), que inclui tanto as áreas finalizadas quanto as não finalizadas. Essa coluna fornece uma medida do espaço total disponível no porão da casa, independentemente de estar ou não finalizado.

Em resumo:

* **`TotalBsmtSF`** = Área finalizada do porão (Tipo 1) + Área finalizada do porão (Tipo 2) + Área não finalizada do porão

Essa informação é útil para avaliar o espaço total que pode ser utilizado na casa, incluindo a possibilidade de conversão de áreas não finalizadas em espaços habitáveis no futuro.

Exemplo:

* Se **`TotalBsmtSF`** for 1.200, isso significa que a área total do porão é de 1.200 pés quadrados (aproximadamente 111,5 metros quadrados), somando todas as partes, tanto acabadas quanto não acabadas.

## **1stFlrSF**

A coluna **`1stFlrSF`** no dataset refere-se à **área do primeiro andar** da casa em  **pés quadrados** . Esta coluna indica a metragem quadrada do espaço habitável no primeiro nível do imóvel, que é normalmente o andar principal, onde se encontram as áreas comuns, como salas de estar, cozinhas, banheiros e, possivelmente, alguns quartos.

É importante notar que essa medida não inclui a área do porão, do segundo andar ou de qualquer outro nível; refere-se exclusivamente à área do primeiro andar.

Exemplo:

* Se **`1stFlrSF`** for 1.500, isso significa que a área do primeiro andar é de 1.500 pés quadrados (aproximadamente 139,4 metros quadrados).

## **2ndFlrSF**

A coluna **`2ndFlrSF`** no dataset refere-se à **área do segundo andar** da casa em  **pés quadrados** . Esta coluna indica a metragem quadrada do espaço habitável no segundo nível do imóvel, que normalmente contém quartos, banheiros e, em alguns casos, áreas de estar ou escritórios.

Assim como  **`1stFlrSF`** , a medida da **`2ndFlrSF`** se concentra apenas no espaço do segundo andar, sem incluir áreas do primeiro andar, do porão ou de outros níveis.

Exemplo:

* Se **`2ndFlrSF`** for 800, isso significa que a área do segundo andar é de 800 pés quadrados (aproximadamente 74,3 metros quadrados).

## **LowQualFinSF**

A coluna **`LowQualFinSF`** no dataset refere-se à **área em pés quadrados** de espaços que foram finalizados, mas com **qualidade baixa** ( *Low Quality Finished Square Feet* ). Essa medida inclui áreas dentro da casa que foram terminadas, mas não atendem aos padrões de qualidade geralmente esperados, como acabamentos inferiores, materiais de baixa qualidade ou características não desejáveis.

Esses espaços podem ser, por exemplo, áreas de porão, sótãos ou extensões que foram concluídas, mas que não têm a mesma qualidade de acabamentos que as áreas normais da casa.

Exemplo:

* Se **`LowQualFinSF`** for 200, isso significa que há 200 pés quadrados (aproximadamente 18,6 metros quadrados) de área finalizada na casa que é considerada de baixa qualidade.

## **GrLivArea**

A coluna **`GrLivArea`** no dataset refere-se à **área de estar acima do nível do solo** (em pés quadrados), que inclui todos os espaços habitáveis da casa que estão acima do nível do solo, ou seja, a soma das áreas dos andares habitáveis.

Isso normalmente inclui a área do primeiro andar e a área do segundo andar, mas não inclui a área do porão, do sótão ou de áreas externas, como garagens ou varandas.

Em resumo:

* **`GrLivArea`** = Área total de estar acima do solo (excluindo porão e sótão).

Exemplo:

* Se **`GrLivArea`** for 1.800, isso significa que a área total de estar acima do solo é de 1.800 pés quadrados (aproximadamente 167,2 metros quadrados). Essa informação é útil para avaliar o espaço habitável real da propriedade.

## **BsmtFullBath**

A coluna **`BsmtFullBath`** no dataset refere-se ao número de **banheiros completos** localizados no porão da casa. Um banheiro completo é definido como aquele que contém pelo menos uma pia, um vaso sanitário e uma ducha ou banheira.

Portanto, **`BsmtFullBath`** conta quantos desses banheiros completos estão disponíveis no espaço do porão.

Exemplo:

* Se **`BsmtFullBath`** for 1, isso significa que há um banheiro completo no porão da casa. Se for 0, significa que não há banheiros completos no porão.

## **BsmtHalfBath**

A coluna **`BsmtHalfBath`** no dataset refere-se ao número de **banheiros meia-banho** localizados no porão da casa. Um banheiro meia-banho é definido como aquele que contém pelo menos uma pia e um vaso sanitário, mas não possui ducha ou banheira.

Portanto, **`BsmtHalfBath`** conta quantos desses banheiros meia-banho estão disponíveis no espaço do porão.

Exemplo:

* Se **`BsmtHalfBath`** for 1, isso significa que há um banheiro meia-banho no porão da casa. Se for 0, significa que não há banheiros meia-banho no porão.

## **FullBath**

A coluna **`FullBath`** no dataset refere-se ao número de **banheiros completos** localizados **acima do nível do solo** na casa. Um banheiro completo é definido como aquele que contém pelo menos uma pia, um vaso sanitário e uma ducha ou banheira.

Portanto, **`FullBath`** conta quantos desses banheiros completos estão disponíveis em todos os andares da casa, excluindo os banheiros do porão.

Exemplo:

- Se **`FullBath`** for 2, isso significa que há dois banheiros completos na casa, localizados em andares acima do solo. Se for 0, significa que não há banheiros completos em nenhum dos andares acima do solo.

## **HalfBath**

A coluna **`HalfBath`** no dataset refere-se ao número de **banheiros meia-banho** localizados **acima do nível do solo** na casa. Um banheiro meia-banho é definido como aquele que contém pelo menos uma pia e um vaso sanitário, mas não possui ducha ou banheira.

Portanto, **`HalfBath`** conta quantos desses banheiros meia-banho estão disponíveis em todos os andares da casa, excluindo os banheiros do porão.

Exemplo:

- Se **`HalfBath`** for 1, isso significa que há um banheiro meia-banho na casa, localizado em um andar acima do solo. Se for 0, significa que não há banheiros meia-banho em nenhum dos andares acima do solo.

## **BedroomAbvGr**

A coluna **`BedroomAbvGr`** no dataset refere-se ao número de **quartos acima do nível do solo** na casa. Essa coluna conta quantos quartos existem em andares que estão acima do solo, excluindo os quartos localizados no porão.

**Exemplo:**

- Se **`BedroomAbvGr`** for 3, isso significa que há três quartos localizados em andares acima do nível do solo. Se for 0, significa que não há quartos acima do nível do solo na casa.

## **KitchenAbvGr**

A coluna **`KitchenAbvGr`** no dataset refere-se ao número de **cozinhas acima do nível do solo** na casa. Essa coluna conta quantas cozinhas estão localizadas em andares que estão acima do solo, excluindo qualquer cozinha que possa estar no porão.

**Exemplo:**

- Se **`KitchenAbvGr`** for 1, isso significa que há uma cozinha localizada em um andar acima do nível do solo. Se for 0, significa que não há cozinhas acima do nível do solo na casa.

## **TotRmsAbvGrd**

A coluna **`TotRmsAbvGrd`** no dataset refere-se ao **número total de cômodos acima do nível do solo**, incluindo todos os tipos de cômodos, exceto banheiros. Isso significa que essa coluna conta todos os cômodos que estão acima do nível do solo, como salas de estar, salas de jantar, quartos e cozinhas, mas não inclui banheiros (tanto completos quanto meia-banho).

**Exemplo:**

- Se **`TotRmsAbvGrd`** for 5, isso significa que há cinco cômodos acima do nível do solo na casa. Se houver 3 quartos, 1 sala de estar e 1 sala de jantar, a soma total será 5.

## **Fireplaces**

A coluna **`Fireplaces`** no dataset refere-se ao número de **lareiras** na casa. Essa coluna conta quantas lareiras estão presentes, independentemente de estarem em andares acima do nível do solo ou no porão.

**Exemplo:**

- Se **`Fireplaces`** for 2, isso significa que há duas lareiras na casa. Se for 0, significa que não há lareiras.

## **GarageYrBlt**

A coluna **`GarageYrBlt`** no dataset refere-se ao **ano em que a garagem foi construída**. Essa coluna fornece informações sobre a data de construção da garagem associada à propriedade.

**Exemplo:**

- Se **`GarageYrBlt`** for 1995, isso significa que a garagem foi construída em 1995. Se o valor for NaN (não disponível), isso pode indicar que a casa não tem garagem ou que a informação não está registrada.

## **GarageCars**

A coluna **`GarageCars`** no dataset refere-se ao **número de carros que a garagem pode acomodar**. Essa coluna indica a capacidade da garagem em termos de quantos veículos ela pode abrigar.

**Exemplo:**

- Se **`GarageCars`** for 2, isso significa que a garagem pode acomodar até dois carros. Se for 0, isso indica que não há garagem ou que a garagem não é capaz de abrigar nenhum carro.

## **GarageArea**

A coluna **`GarageArea`** no dataset refere-se à **área da garagem em pés quadrados** (square feet). Essa coluna fornece informações sobre o tamanho total da garagem, medindo sua área disponível para estacionar veículos ou para uso como espaço adicional.

**Exemplo:**

- Se **`GarageArea`** for 400, isso significa que a área total da garagem é de 400 pés quadrados. Se for 0, pode indicar que não há garagem ou que a informação não está disponível.

## **WoodDeckSF**

A coluna **`WoodDeckSF`** no dataset refere-se à **área do deck de madeira em pés quadrados** (square feet). Essa coluna fornece informações sobre o tamanho do espaço externo de madeira, que pode ser usado para entretenimento, lazer ou atividades ao ar livre.

**Exemplo:**

- Se **`WoodDeckSF`** for 150, isso significa que a área do deck de madeira é de 150 pés quadrados. Se o valor for 0, significa que não há deck de madeira presente na propriedade.

## **OpenPorchSF**

A coluna **`OpenPorchSF`** no dataset refere-se à **área do alpendre aberto em pés quadrados** (square feet). Essa coluna fornece informações sobre o tamanho do espaço externo coberto, mas que não é fechado, que pode ser usado para relaxamento, entretenimento ou como uma entrada adicional para a casa.

**Exemplo:**

- Se **`OpenPorchSF`** for 100, isso significa que a área do alpendre aberto é de 100 pés quadrados. Se o valor for 0, indica que não há alpendre aberto na propriedade.

## **EnclosedPorch**

A coluna **`EnclosedPorch`** no dataset refere-se à **área do alpendre fechado em pés quadrados** (square feet). Essa coluna fornece informações sobre o tamanho do espaço externo que é coberto e fechado, oferecendo um ambiente interno adicional que pode ser usado como sala, escritório ou área de estar.

**Exemplo:**

- Se **`EnclosedPorch`** for 50, isso significa que a área do alpendre fechado é de 50 pés quadrados. Se o valor for 0, indica que não há alpendre fechado presente na propriedade.

## **3SsnPorch**

A coluna **`3SsnPorch`** no dataset refere-se à **área do alpendre de três estações em pés quadrados** (square feet). Um alpendre de três estações é um espaço que geralmente é coberto e fechado, mas não é totalmente aquecido. É um local que pode ser utilizado em várias estações do ano, proporcionando uma transição entre o interior e o exterior da casa.

**Exemplo:**

- Se **`3SsnPorch`** for 120, isso significa que a área do alpendre de três estações é de 120 pés quadrados. Se o valor for 0, indica que não há alpendre de três estações presente na propriedade.

## **ScreenPorch**

A coluna **`ScreenPorch`** no dataset refere-se à **área do alpendre com tela em pés quadrados** (square feet). Um alpendre com tela é um espaço externo coberto que possui telas em vez de paredes, proporcionando proteção contra insetos e permitindo a circulação de ar. É um local que pode ser utilizado para relaxamento e entretenimento ao ar livre.

**Exemplo:**

- Se **`ScreenPorch`** for 80, isso significa que a área do alpendre com tela é de 80 pés quadrados. Se o valor for 0, indica que não há alpendre com tela presente na propriedade.

## **PoolArea**

A coluna **`PoolArea`** no dataset refere-se à **área da piscina em pés quadrados** (square feet). Essa coluna fornece informações sobre o tamanho da área da piscina em uma propriedade, indicando o espaço dedicado a essa instalação.

**Exemplo:**

- Se **`PoolArea`** for 200, isso significa que a área da piscina é de 200 pés quadrados. Se o valor for 0, indica que não há piscina na propriedade.

## **MiscVal**

A coluna **`MiscVal`** no dataset refere-se ao **valor em dólares de recursos ou características diversas que não estão cobertos em outras categorias**. Isso pode incluir características ou melhorias especiais que não se enquadram nas classificações padrão de atributos da casa, como um gazebo, uma estufa ou qualquer outra melhoria que possa ter um valor monetário associado.

**Exemplo:**

- Se **`MiscVal`** for 5000, isso significa que o valor das características diversas associadas à propriedade é de 5.000 dólares. Se o valor for 0, indica que não há recursos ou características especiais que contribuam para o valor da propriedade.

## **MoSold**

A coluna **`MoSold`** no dataset refere-se ao **mês em que a propriedade foi vendida**. Essa coluna é representada como um número inteiro que varia de 1 a 12, correspondendo aos meses do ano. Essa informação pode ser útil para análise sazonal das vendas de propriedades.

**Exemplo:**

- Se **`MoSold`** for 6, isso significa que a propriedade foi vendida em junho.

## **YrSold**

A coluna **`YrSold`** no dataset refere-se ao **ano em que a propriedade foi vendida**. Essa coluna é representada como um número inteiro que indica o ano da transação. Informações sobre o ano de venda podem ser valiosas para análises de tendências no mercado imobiliário ao longo do tempo.

**Exemplo:**

- Se **`YrSold`** for 2010, isso significa que a propriedade foi vendida no ano de 2010.

## **SalePrice**

A coluna **`SalePrice`** no dataset refere-se ao **preço de venda da propriedade em dólares**. Esta é a variável alvo que você está tentando prever ao construir um modelo de regressão. O **`SalePrice`** é um dos dados mais importantes para análise de mercado e avaliação de propriedades.

**Exemplo:**

- Se **`SalePrice`** for 250000, isso significa que a propriedade foi vendida por 250.000 dólares.

## **MSZoning**

A coluna **`MSZoning`** no dataset refere-se à **classificação de zoneamento geral da propriedade**. Ela indica o uso permitido da propriedade de acordo com a regulamentação de zoneamento da área. As categorias podem incluir zonas residenciais, comerciais, industriais e outras, que determinam como a terra pode ser utilizada.

**Exemplo de categorias comuns em `MSZoning`:**

- **RL**: Residencial de baixa densidade (Low Density Residential)
- **RM**: Residencial de média densidade (Medium Density Residential)
- **C**: Comercial (Commercial)
- **FV**: Zona de uso variado (Floating Village)
- **I**: Industrial (Industrial)

Essas informações são importantes para entender as restrições e possibilidades de desenvolvimento de cada propriedade.

## **Street**

A coluna **`Street`** no dataset refere-se ao **tipo de acesso rodoviário da propriedade**. Ela indica a qualidade e o tipo da rua em que a propriedade está localizada. Os valores nesta coluna geralmente classificam as ruas em diferentes categorias, que podem impactar o valor da propriedade e o acesso aos serviços.

**Exemplo de categorias em `Street`:**

- **Grvl**: Rua de cascalho (Gravel)
- **Pave**: Rua pavimentada (Paved)

Essas informações podem ser úteis para análises relacionadas à acessibilidade e infraestrutura do bairro.

## **Alley**

A coluna **`Alley`** no dataset refere-se ao **tipo de acesso à viela ou alley da propriedade**. As vielas são ruas menores que geralmente não são usadas para tráfego principal, mas podem fornecer acesso a áreas traseiras de propriedades.

**Exemplo de categorias em `Alley`:**

- **Grvl**: Viela de cascalho (Gravel)
- **Pave**: Viela pavimentada (Paved)
- **NA**: Sem acesso à viela (No alley access)

A informação sobre o acesso à viela pode ser relevante para avaliações de propriedades e considerações sobre privacidade e espaço adicional.

## **LotShape**

A coluna **`LotShape`** no dataset refere-se à **forma geral do lote** em que a propriedade está situada. Essa informação pode influenciar a construção, o uso do espaço e, consequentemente, o valor da propriedade.

**Exemplo de categorias em `LotShape`:**

- **Reg**: Lote regular (Regular) — Lote com forma retangular ou quadrada.
- **IR1**: Lote irregular (Irregular 1) — Lote com uma forma levemente irregular.
- **IR2**: Lote irregular (Irregular 2) — Lote com uma forma mais irregular.
- **Lshaped**: Lote em forma de L (L-shaped) — Lote que tem uma forma semelhante à letra "L".

Essas características podem afetar a construção e o planejamento do uso da propriedade, além de influenciar a avaliação do valor do imóvel.

## **LandContour**

A coluna **`LandContour`** no dataset refere-se à **topografia ou contorno do terreno** em que a propriedade está localizada. Isso pode incluir informações sobre a planicidade do terreno, que pode impactar a construção, a drenagem e outros fatores relevantes para o valor da propriedade.

**Exemplo de categorias em `LandContour`:**

- **Lvl**: Terreno plano (Level) — O terreno é relativamente plano, sem inclinações significativas.
- **Bnk**: Terreno em declive (Bank) — O terreno é inclinado, como uma encosta.
- **HLS**: Terreno em encosta (Hillside) — O terreno é uma área montanhosa ou em colina.
- **Low**: Terreno em área baixa (Low) — O terreno está em uma área baixa, que pode ser suscetível a inundações.

A topografia do terreno pode influenciar a construção e a acessibilidade da propriedade, além de ter um impacto direto na avaliação de seu valor.

## **Utilities**

A coluna **`Utilities`** no dataset refere-se ao **tipo de utilidades disponíveis** na propriedade. Essa informação é importante porque a disponibilidade de serviços públicos pode impactar tanto a habitabilidade quanto o valor da propriedade.

**Exemplo de categorias em `Utilities`:**

- **AllPub**: Todas as utilidades públicas disponíveis (All Public Utilities) — A propriedade tem acesso a todas as utilidades, incluindo água, esgoto, eletricidade e gás.
- **NoSewr**: Sem esgoto público (No Sewer) — A propriedade não tem acesso ao sistema de esgoto público.
- **NoSeWa**: Sem serviços públicos (No Sewer and Water) — A propriedade não tem acesso a água ou esgoto públicos.
- **ELO**: Somente eletricidade (Electricity Only) — A propriedade tem apenas acesso à eletricidade.

A disponibilidade de utilidades pode influenciar a decisão de compra e o valor de mercado de uma propriedade.


## **LotConfig**

A coluna **`LotConfig`** no dataset refere-se à **configuração do lote** da propriedade, o que pode afetar o uso do terreno e, consequentemente, seu valor. Essa informação é relevante para entender como a propriedade se relaciona com outras propriedades vizinhas e como o espaço pode ser utilizado.

**Exemplo de categorias em `LotConfig`:**

- **Inside**: Lote interno — O lote está localizado no interior de um bloco, longe de ruas principais ou de esquina.
- **Corner**: Lote de esquina — O lote está situado na interseção de duas ruas, oferecendo acesso em dois lados.
- **CulDSac**: Lote em cul-de-sac — O lote está localizado em uma rua sem saída, geralmente em uma área tranquila.
- **FR2**: Lote com frente dupla — O lote tem dois lados com frente para ruas.
- **FR3**: Lote com frente tripla — O lote tem três lados com frente para ruas.

A configuração do lote pode influenciar a acessibilidade, o potencial de desenvolvimento e a privacidade da propriedade, impactando seu valor de mercado.


## **LandSlope**

A coluna **`LandSlope`** no dataset refere-se à **inclinação do terreno** da propriedade, que pode afetar a construção, a drenagem e o uso do solo. Essa informação é relevante para entender as características físicas do terreno e como elas podem impactar o valor da propriedade e a habitabilidade.

**Exemplo de categorias em `LandSlope`:**

- **Gtl (Gentle Slope)**: Inclinação suave — O terreno tem uma leve inclinação, facilitando a construção e a drenagem.
- **Mod (Moderate Slope)**: Inclinação moderada — O terreno tem uma inclinação mais acentuada, o que pode exigir considerações adicionais para construção e drenagem.
- **Sev (Severe Slope)**: Inclinação acentuada — O terreno é bastante inclinado, o que pode representar desafios significativos para construção, drenagem e uso.

A inclinação do terreno pode influenciar decisões relacionadas à construção, ao paisagismo e à acessibilidade, impactando, assim, o valor da propriedade.


## **Neighborhood**

A coluna **`Neighborhood`** no dataset refere-se à **localização física da propriedade dentro dos limites da cidade de Ames**. Essa informação é crucial porque diferentes bairros podem ter características distintas que afetam o valor da propriedade, como a qualidade das escolas, a proximidade de serviços e a segurança.

**Importância do `Neighborhood`:**

- **Valorização**: Bairros diferentes podem ter faixas de preço muito distintas, influenciando diretamente o valor de venda da propriedade.
- **Infraestrutura e serviços**: Acesso a parques, transporte público, comércio e serviços pode variar de um bairro para outro.
- **Qualidade de vida**: Algumas áreas podem ser mais tranquilas ou ter uma comunidade mais ativa, o que pode ser um fator decisivo para potenciais compradores.

**Exemplo de categorias em `Neighborhood`:**

- **CollgCr**: College Creek
- **Veenker**: Veenker
- **Crawfor**: Crawford
- **NoRidge**: North Ridge
- **OldTown**: Old Town
- **Sawyer**: Sawyer
- **Somerst**: Somerset
- **Edwards**: Edwards

Cada um desses bairros pode ter características únicas que influenciam a percepção de valor e o interesse de compradores em potencial.

## **Condition1**

A coluna **`Condition1`** no dataset refere-se à **proximidade da propriedade a uma estrada principal ou ferrovia**. Essa informação é importante, pois a localização em relação a essas vias pode afetar o valor da propriedade, a qualidade de vida dos moradores e a percepção geral da área.

### Significado e Importância de `Condition1`:

- **Avaliação de Ruído**: Propriedades localizadas próximas a rodovias ou ferrovias podem ser mais barulhentas, o que pode impactar a qualidade de vida.
- **Acesso e Comodidade**: A proximidade a estradas principais pode oferecer melhor acesso a transporte, serviços e comércio, tornando a propriedade mais atraente.
- **Valorização**: As propriedades em áreas mais tranquilas, longe de grandes vias, geralmente têm um valor mais alto devido à busca por ambientes residenciais mais calmos.

### Exemplo de categorias em `Condition1`:

- **Artery**: Propriedade adjacente a uma estrada principal.
- **Feederv**: Propriedade adjacente a uma via de serviço ou secundária.
- **Normal**: Propriedade em uma localização padrão, sem influência significativa de tráfego.
- **RRAe**: Propriedade em uma área de ferrovia.
- **RRNn**: Propriedade em uma área de ferrovia, mas com menor impacto do ruído.

Essas categorias ajudam a descrever as condições de localização da propriedade e podem ser fatores importantes na avaliação de imóveis.


## **Condition2**

A coluna **`Condition2`** no dataset também se refere à **proximidade da propriedade a uma estrada principal ou ferrovia**, mas é usada para indicar uma segunda condição se a propriedade estiver próxima de mais de uma dessas vias.

### Significado e Importância de `Condition2`:

- **Proximidade Dupla**: Essa coluna é útil para identificar propriedades que podem estar sob a influência de múltiplas fontes de ruído ou tráfego. Se uma propriedade estiver próxima de uma estrada principal e uma ferrovia, isso pode impactar ainda mais o valor e a qualidade de vida.
- **Aumento de Ruído e Tráfego**: Propriedades que se encontram em condições de proximidade dupla podem ser mais suscetíveis a barulho e tráfego intenso, o que pode influenciar negativamente a percepção do comprador.
- **Análise Mais Detalhada**: A inclusão dessa coluna permite uma análise mais aprofundada do impacto das condições ambientais e de tráfego na valorização das propriedades.

### Exemplo de categorias em `Condition2`:

- **Artery**: Propriedade adjacente a uma estrada principal.
- **Feederv**: Propriedade adjacente a uma via de serviço ou secundária.
- **Normal**: Propriedade em uma localização padrão, sem influência significativa de tráfego.
- **RRAe**: Propriedade em uma área de ferrovia.
- **RRNn**: Propriedade em uma área de ferrovia, mas com menor impacto do ruído.
- **Pos**: Propriedade com acesso a uma via secundária.

Essas categorias ajudam a oferecer uma visão mais clara das condições em que a propriedade se encontra, permitindo uma melhor avaliação de seu valor de mercado.


## **BldgType**

A coluna **`BldgType`** no dataset refere-se ao **tipo de edifício** da propriedade. Essa informação é importante porque diferentes tipos de edifícios podem ter características distintas que afetam seu valor, layout e uso.

### Significado e Importância de `BldgType`:

- **Classificação dos Edifícios**: `BldgType` categoriza os edifícios em diferentes tipos, que podem incluir, mas não se limitam a:

  - **1Fam**: Residência unifamiliar (uma única casa).
  - **2FmCon**: Casa bifamiliar (duas unidades em uma única estrutura).
  - **Duplex**: Edifício dividido em duas unidades.
  - **Twnhs**: Townhouse (casas geminadas).
  - **TwnhsE**: Townhouse em extremidade (casas geminadas com uma extremidade livre).
  - **Row**: Edifícios em fila (várias unidades conectadas em uma linha).
- **Impacto no Valor**: O tipo de edifício pode influenciar o preço de venda. Por exemplo, uma casa unifamiliar pode ter um valor de mercado diferente em comparação com um townhouse devido ao espaço, privacidade e amenidades associadas a cada tipo.
- **Análise de Mercado**: Compreender o tipo de edifício pode ajudar a identificar tendências de mercado em áreas específicas e a determinar quais tipos de propriedades são mais desejáveis em um determinado momento.
- **Características de Design e Estrutura**: Cada tipo de edifício pode ter características de design e estrutura que são relevantes para a avaliação da condição e do valor da propriedade.

A análise dessa coluna é fundamental para entender como o tipo de edifício se relaciona com outras variáveis e o preço de venda da propriedade.


## HouseStyle

A coluna **`HouseStyle`** no dataset se refere ao **estilo arquitetônico da residência**. Essa informação é importante porque o estilo da casa pode influenciar o valor de mercado, a atratividade e as características gerais da propriedade.

### Significado e Categorias de `HouseStyle`:

- **1Story**: Casa de um andar - uma residência com apenas um nível.
- **1.5Story**: Casa de um andar e meio - uma residência que possui um andar principal e um segundo nível que é parcialmente usado.
- **2Story**: Casa de dois andares - uma residência com dois níveis completos.
- **2.5Story**: Casa de dois andares e meio - similar à casa de dois andares, mas com um sótão ou espaço adicional no andar superior.
- **SplitFoyer**: Casa com entrada dividida - uma residência em que a entrada principal leva a um nível inferior e a um nível superior, com escadas em ambas as direções.
- **SplitLevel**: Casa de nível dividido - uma residência com diferentes níveis de piso, geralmente com um pequeno número de escadas entre os níveis.
- **Duplex**: Edifício que contém duas unidades residenciais.
- **Twnhs**: Townhouse - uma casa geminada que faz parte de uma fileira de casas conectadas.

### Importância de `HouseStyle`:

- **Valoração**: O estilo da casa pode influenciar o preço de venda. Estilos mais populares ou desejáveis podem ter preços mais altos.
- **Características e Layout**: Diferentes estilos de casas podem ter layouts e características distintas, como o número de quartos, banheiros e áreas de estar, que afetam a funcionalidade e o conforto da residência.
- **Preferências do Comprador**: O estilo arquitetônico pode refletir as preferências do comprador, e a análise dessa coluna pode ajudar a entender quais estilos estão em alta no mercado.

Entender a coluna `HouseStyle` pode ser fundamental para a análise de como o estilo da casa se relaciona com o preço de venda e outras variáveis no dataset.
