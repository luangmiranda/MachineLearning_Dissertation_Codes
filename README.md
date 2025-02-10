
# Dissertação de Mestrado: Detecção de Anomalias em Redes Utilizando Autoencoders

Neste projeto são apresentados os códigos desenvolvidos no desenvolvimento da Dissertação apresentada no curso de Mestrado em Engenharia da Informação da UFABC.

## Resumo

Nas últimas décadas, houve um aumento significativo de dispositivos e sistemas conectados à internet, o que exige uma evolução contínua das estratégias de segurança cibernética devido à sensibilidade dos dados transmitidos por essas redes.
Dentre as estratégias emergentes, os sistemas de detecção de intrusão têm ganhado destaque, particularmente uma subclasse chamada de sistema de detecção de anomalia (ADS, do inglês Anomaly Detection System), que detecta ameaças ao identificar anomalias em relação aos dados de tráfego normais da rede. A importância dos ADSs reside na capacidade de identificar ataques desconhecidos sem a necessidade de conhecimento prévio das suas características.

Uma possível implementação de um ADS que vêm sendo investigada é a que faz uso de algoritmos de aprendizado de máquina (ML, do inglês Machine Learning).
No entanto, estes algoritmos precisam de dados para o seu treinamento e é comum que dados de ataque estejam em um número menor que dados de tráfego normais, o que pode enviesar esses algoritmos.
Assim, auto codificadores (AE, do inglês Autoencoder) têm sido empregados pelo fato de ser possível treiná-los com os dados de apenas uma classe, geralmente a majoritária.
Parâmetros extraídos do AE, como o erro de reconstrução (RE, do inglês Reconstruction Error), podem ser utilizados para distinguir os dados normais de dados de ataques, o que geralmente é feito comparando-o com um limiar.
A obtenção deste limiar pode ser feita através de diferentes critérios e depende geralmente de parâmetros que não são conhecidos e que precisam ser estimados.
Exemplos desses parâmetros vão desde valores simples, como média e variância, até funções mais complicadas, como distribuições de probabilidade e momentos estatísticos de ordens superiores.

Esta dissertação, portanto, propõe uma estrutura conjunta de um AE e um classificador, com o classificador substituindo os limiares clássicos.
O uso de um classificador para a detecção abre a possibilidade de se incluir outras características que podem ser obtidas com o AE, como os valores da camada intermediária, visando melhorar a detecção dos ataques.
Nesta dissertação, diversos cenários foram avaliados, combinando diferentes classificadores como o KNN, DT e SVM,  e diferentes combinações de características.
Os resultados obtidos mostraram uma melhora na detecção de ataques em grande parte dos cenários ao se utilizar a estrutura proposta, em especial utilizando o KNN.

## Divisão do projeto
Neste projeto foram utilizados 3 datasets diferentes: NSL-KDD, BOT-IOT e CIC-IDS2017. Com isso, os códigos desenvolvidos para cada dataset é apresentado dentro da pasta com o respectivo nome.

## Sites
www.ufabc.edu.br

propg.ufabc.edu.br/ppginfo

## 
O presente trabalho foi realizado com apoio da Coordenacão de Aperfeiçoamento de
Pessoal de Nível Superior – Brasil (CAPES) – Código de Financiamento 001



