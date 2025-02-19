# ConcursoApp

Este projeto é uma aplicação em Java para carregar dados de candidatos a um concurso a partir de um arquivo CSV, ordená-los com base na nota e na idade (em caso de empate de nota), e exibir o resultado ordenado.

## Funcionalidades

- Carregamento de dados de candidatos de um arquivo CSV.
- Ordenação de candidatos com base na nota em ordem decrescente.
- Desempate por idade (candidatos mais velhos ficam melhor classificados).
- Exibição dos candidatos em ordem após a classificação.


## Formato do Arquivo CSV

O arquivo CSV deve conter as seguintes colunas, separadas por tabulação:

- **Identificador**: Número único do candidato.
- **Nome**: Nome completo do candidato.
- **Data de Nascimento**: Data de nascimento no formato `dd/MM/yyyy`.
- **Nota**: Nota do candidato no concurso (inteiro).

Exemplo de arquivo CSV:

[Uploading dadIdentificador,Nome,Data de Nascimento,Nota
1,Alice Silva,01/01/1980,50
2,Miguel Santos,02/02/1985,65
3,Sophia Oliveira,03/03/1990,70
4,Arthur Rodrigues,04/04/1982,88
5,Helena Costa,05/05/1995,88
6,Heitor Gomes,06/06/1988,43
7,Laura Pereira,07/07/1991,67
8,Bernardo Ribeiro,08/08/1983,91
9,Valentina Almeida,09/09/1998,23
10,Davi Cunha,10/10/1986,23
11,Isabella Campos,11/11/1989,55
12,Lorenzo Cardoso,12/12/1992,79
13,Manuela Lima,13/01/1984,90
14,Joao Souza,14/02/1997,32
15,Heloisa Teixeira,15/03/1981,32
16,Theo Fernandes,16/04/1994,66
17,Liz Ferreira,17/05/1987,81
18,Caua Lopes,18/06/1990,19
19,Lorena Martins,19/07/1985,45
20,Benjamin Garcia,20/08/1993,45
21,Cecilia Moraes,21/09/1988,78
22,Rafael Barbosa,22/10/1996,34
23,Lavinia Nascimento,23/11/1982,59
24,Enzo Araujo,24/12/1999,89
25,Maria Pinto,25/01/1986,89
26,Joao Miguel Freitas,26/02/1991,40
27,Ana Clara Barros,27/03/1989,72
28,Pedro Henrique Santos,28/04/1994,21
29,Clara Vitoria Castro,29/05/1983,53
30,Anthony Tomás Guimarães,30/06/1997,53
31,Maite Correia,01/07/1987,93
32,Nicolas Vicente,02/08/1990,35
33,Antonella Nogueira,03/09/1985,68
34,Felipe Rocha,04/10/1993,10
35,Melissa Miranda,05/11/1981,10
36,Samuel Gonçalves,06/12/1996,77
37,Emily Dias,07/01/1989,29
38,Davi Lucas Oliveira,08/02/1992,61
39,Agatha Farias,09/03/1987,97
40,Pietro Ribeiro,10/04/1995,97
41,Ester Fernandes,11/05/1984,38
42,Enrico Pereira,12/06/1998,70
43,Sophie Alves,13/07/1982,18
44,Augusto Costa,14/08/1991,51
45,Luna Carvalho,15/09/1989,51
46,Levi Gomes,16/10/1994,83
47,Ayla Rodrigues,17/11/1983,26
48,Benicio Cunha,18/12/1997,64
49,Elisa Almeida,19/01/1986,95
50,Henry Campos,20/02/1990,95
51,Melissa Cardoso,21/03/1989,46
52,Bryan Lima,22/04/1993,79
53,Mariah Souza,23/05/1987,16
54,Gabriel Teixeira,24/06/1991,49
55,Alice Lopes,25/07/1985,49
56,Arthur Martins,26/08/1994,87
57,Livia Garcia,27/09/1988,30
58,Bernardo Moraes,28/10/1992,63
59,Valentina Barbosa,29/11/1986,99
60,Davi Nascimento,30/12/1990,99
61,Isabella Araujo,01/01/1984,41
62,Lorenzo Pinto,02/02/1993,74
63,Manuela Freitas,03/03/1988,12
64,Joao Barros,04/04/1996,45
65,Heloisa Santos,05/05/1982,45
66,Theo Castro,06/06/1990,86
67,Liz Guimaraes,07/07/1985,28
68,Caua Correia,08/08/1993,61
69,Lorena Vicente,09/09/1989,98
70,Benjamin Nogueira,10/10/1997,98
71,Cecilia Rocha,11/11/1983,39
72,Rafael Miranda,12/12/1991,72
73,Lavinia Gonçalves,13/01/1987,10
74,Pedro Dias,14/02/1995,43
75,Maria Oliveira,15/03/1999,43
76,Joao Miguel Farias,16/04/1983,80
77,Ana Clara Ribeiro,17/05/1996,24
78,Pedro Henrique Fernandes,18/06/1989,57
79,Clara Vitoria Pereira,19/07/1992,96
80,Anthony Alves,20/08/1987,96
81,Maite Costa,21/09/1990,37
82,Nicolas Carvalho,22/10/1994,71
83,Antonella Gomes,23/11/1981,08
84,Felipe Rodrigues,24/12/1997,41
85,Melissa Cunha,25/01/1985,41
86,Samuel Almeida,26/02/1991,84
87,Emily Campos,27/03/1988,27
88,Davi Lucas Cardoso,28/04/1994,59
89,Agatha Lima,29/05/1982,93
90,Pietro Souza,30/06/1996,93
91,Ester Teixeira,01/07/1989,36
92,Enrico Fernandes,02/08/1993,69
93,Sophie Pereira,03/09/1986,07
94,Augusto Alves,04/10/1990,39
95,Luna Costa,05/11/1994,39
96,Levi Carvalho,06/12/1987,82
97,Ayla Gomes,07/01/1991,25
98,Benicio Rodrigues,08/02/1984,58
99,Elisa Cunha,09/03/1998,97
100,Henry Almeida,10/04/1982,97osConcurso.csv…]()
