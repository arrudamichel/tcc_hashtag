# Uma ferramenta de análise de padrões em hashtags no Twitter

Trabalho apresentado para a conclusão do curso de graduação em Bacharelado em Ciência da Computação pela Universidade Federal Rural do Rio de Janeiro, por Michel Arruda e Rafael Costa e orientado por Carlos Eduardo Mello.

Texto final em: "texto_final_tcc.pdf"

Apresentação final em: "apresentacao_final_tcc.pptx"

## Resumo

Neste trabalho, uma solução de mineração de dados é desenvolvida cujo objetivo consiste na descoberta de padrões em hashtags a partir de dados do Twitter. Inicialmente, pode ser vista uma comparação entre algumas ferramentas similares encontradas na Internet, onde uma carência por ferramentas de mineração de da-
dos em hashtags pode ser notada. Tal carência se torna alarmante devido à grande quantidade de dados oriundos de redes sociais, a qual inviabiliza a identificação de padrões por um processo de análise manual, e então, tornando-se necessária a criação desta solução.


Para tal, etapas de processamento que consistem na execução sequencial de workflows desenvolvidos foram utilizadas, que possibilitam a extração, tratamento, se-
leção, processamento e exibição dos padrões adquiridos. Por fim, a ferramenta foi aplicada a um estudo de caso, onde as hashtags #foraDilma e #foraCunha foram
utilizadas como alvo de busca, apresentando resultados satisfatórios. A partir dos resultados, foi possível visualizar a forte ligação entre a presidenta Dilma Rousseff e o seu partido, o PT, além de manifestações de repúdio à presidente. Além disso, pode ser visto que grande parte das manifestações contrárias a Eduardo Cunha ocorreram em virtude do pedido de impeachment da presidente Dilma Rousseff. Tais resultados reforçam a importância da mineração de dados no Twitter e a eficiência da ferramenta criada.


## Workflows

Para implementação da ferramenta, foi utilizado o [Knime](https://www.knime.com/), que provê um ambiente visual para construção de workflows que podem ser utilizados em pipeline de ETL, análise e extração de resultado em dados. 


Foram criados 5 workflows: Obtenção de dados do Twitter, Regra de Associação em Hashtags, Matriz de Distância, Matriz de Coocorrência e Gráfico de Frequência.


Para ter acesso aos workflows, acesse a pasta [/workflow](https://github.com/arrudamichel/tcc_hashtag/edit/master/Workflows/). 


Para importar cada workflow, abra o Knime e acesse "File/Import Knime Workflow..."

#### Obtenção de dados do Twitter

O workflow abaixo apresenta onde é realizada a obtenção dos tweets, extração das hashtags e armazenamento em um banco de dados.

<img src="/Imagens/obtencaoHashtag.png" />

#### Regra de Associação em Hashtags

O workflow abaixo exibe as fases de obtenção dos dados armazenados, de preparação e processamento desses dados.

<img src="/Imagens/regraAssociacao.png" />

#### Matriz de Distância

O workflow abaixo exibe as fases para obtenção, preparação e criação da matriz de distância.

<img src="/Imagens/matrizDistancia.png" />

#### Matriz de Coocorrência

O workflow abaixo exibe as fases para obtenção, preparação e criação da matriz de coocorrência.

<img src="/Imagens/matrizCoocorrencia.png" />

#### Gráfico de Frequência de Hashtags

O workflow abaixo exibe as fases para obtenção, preparação e criação do gráfico de frequência de hashtags.

<img src="/Imagens/graficos.png" />
