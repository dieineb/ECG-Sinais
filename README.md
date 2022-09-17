# ECG-Sinais
Universidade Federal de Ciências da Saúde de Porto Alegre <p>
Dieine Estela Bernieri Schiavon <p>
Porto Alegre, Brasil <p>
dieineb@ufcspa.edu.br <p>
Informática Biomédica - UFCSPA Processamento de Sinais (INF0021)<p>

a)Sinal no domínio do TEMPO: <p>
Pré-processamento do sinal original (bruto):<P>
A entrada bruta do sinal de ECG está sujeita a ruídos principalmente na entrada e saída do
sinal. Muitos artefatos podem inferir ruídos no sinal de ECG. As três fontes mais comuns são:
ruídos de linha de base, interferência da rede elétrica e ruído muscular levando a perdas de
atenuação. Portanto, a remoção do ruído é essencial para uma melhor visualização e análise
do sinal, prevenindo assim erros de interpretação pelo profissional da saúde que irá analisá-lo.<P>
A remoção de ruído no sinal bruto de ECG foi realizada com corte das regiões que
apresentavam ruídos grosseiros no início (≅ 80s) e no final (≅ 780s) do sinal. Outras técnicas
podem ser aplicadas na prática, como por exemplo uso de filtros da mediana.<P>

b) Espectro de amplitude do sinal (com janelas de 3, 5 e 10 segundos):<P>
Após, foi realizada a extração do espectro de amplitude de todo o sinal, já nessa etapa
também foi obtido a maior amplitude (35908) na frequência (2.99Hz) encontrada no sinal.<P>

c) Tipo de ruído presente no sinal:<P>
Ruídos de alta frequência presentes no sinal. Os principais problemas no processamento de
sinais biológicos, tais como o ECG, são a remoção de ruídos. Os ruídos podem ser gerados por
instabilidade de energia (interferência de 60Hz), movimentação corporal, manipulação dos
eletrodos na aplicação e remoção dos mesmos, entre outros. <P>

d) Filtrar o sinal com a transformada de Fourier removendo o ruído:<P>
A próxima etapa é a extração de características. A técnica de transformada rápida de Fourier é
efetivamente introduzida para extrair componentes de características, como sinais PQRST, do sinal
de ECG. Esta técnica irá decompor o sinal original do domínio do tempo para o domínio da
frequência. Sinais de alta frequência e valores máximos de determinada frequência serão
extraídos do domínio da frequência com base na técnica de thresholding. O sinal de ECG original, mesmo pré-processado,
pode conter bastante ruído,então é necessária uma técnica eficiente de filtragem do sinal para remoção de ruídos que
podem comprometer a qualidade do sinal a ser avaliado.<P>

Ampliação da sobreposição e identificação do Complexo QRS nas ondas 1 e 2– Janela de 2 segundos<P>
O sinal foi ampliado, inicialmente em uma janela de cerca de 1 segundo (entre 250 e 250.8 ), na
ampliação, foi evidenciado o complexo QRS <P>

Após a verificação da melhor sobreposição da onda R, foi utilizada uma janela de 2
segundos a fim de obter uma visualização de 2 ondas e consequentemente observar e calcular
o intervalo R-R. O batimento cardíaco do paciente será determinado com o auxílio de
intervalos R-R, que são calculados pela distância entre dois picos R. Este valor do intervalo R-R
também será usado para entender o ritmo cardíaco do paciente.

Referências:<p>
Arquivos Brasileiros de Cardiologia – III Diretrizes da Sociedade Brasileira de Cardiologia Sobre
Análise e emissão de Laudos Eletrocardiográficos. Disponível em
http://publicacoes.cardiol.br/2014/diretrizes/2016/01_III_DIRETRIZES_ELETROCARDIOGR%C3
%81FICOS.pdf. Acesso: 19/08/2021 <p>

B. V. P Prasad & Velusamy Parthasarathy (2018) Detection and classification of cardiovascular
abnormalities using FFT based multi-objective genetic algorithm, Biotechnology &
Biotechnological Equipment, 32:1, 183-193, DOI: 10.1080/13102818.2017.1389303 To link to
this article: https://doi.org/10.1080/13102818.2017.1389303<p>

Conteúdo disponibilizado no moodle da disciplina Processamento de Sinais (Slides, vídeos,
arquivos extensão ipynb, bibliografia sugerida). Professora Regente Dra. Carla Diniz Lopes
Becker <p>

ECGWAVES – POCKET GUIDE TO ECG INTERPRETATION – Disponível em
https://ecgwaves.com/wp-content/uploads/2017/10/Pocket-guide-ECG-interpretation.pdf.
Acesso em 20/08/2021<p>

Estimativa Robusta da Frequência Cardíaca a partir de Sinais de Fotopletismografia de Pulso.
Autor: Tiago Benetti. Disponível em
https://tede2.pucrs.br/tede2/bitstream/tede/8337/2/TIAGO%20BENETTI_DIS.pdf. Acesso:
20/08/2021<p>

Matplotlib Version – Disponível em
https://matplotlib.org/stable/tutorials/text/annotations.html. Acesso em 20/08/2021
Python Data Science Handbook
Disponível em https://jakevdp.github.io/PythonDataScienceHandbook/04.09-text-and-
annotation.html. Acesso em 20/08/2021<p>

SISTEMA DE AQUISIÇÃO DE SINAIS DE EMG E ECG PARA PLATAFORMA ANDROID TM. Autor:
Pedro Victor Eugênio de Souza. Disponível em
https://www.ufpe.br/documents/39830/1359036/259_PedroSouza/9fd3d859-f844-48cd-
99c2-0d5f22b121d6. Acesso em 20/08/2021
