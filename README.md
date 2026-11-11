Caderno de Análise Técnica: IA e Ciência de Dados na Cultura Popular
Aluno(a): [Khemilly Facchetti]
Turma: 1º D — Ensino Médio Técnico Profissionalizante em Inteligência Artificial   
Disciplinas: Ciência de Dados & Técnicas Integradas em IA   
Instituição: Colégio Estadual Rodolpho Zaninelli   
BLOCO 1: Joan é péssima & O Dilema das Redes (Privacidade, Dados e Redes)
Questão 1 [Ciência de Dados]
O pré-processamento de dados utilizando a biblioteca Pandas é uma etapa indispensável antes do treinamento de qualquer modelo de aprendizado de máquina ou sistema de linguagem generativa.
Remoção de Colunas Sensíveis (df.drop): Informações de Identificação Pessoal (PII) — como nomes, CPF, endereços e histórico bancário — atuam como ruído estatístico e violam diretrizes de privacidade e governança de dados (como a LGPD). O uso do comando df.drop(columns=['Nome', 'CPF']) elimina esses atributos antes da fase de modelagem, garantindo que a Inteligência Artificial aprenda apenas padrões gerais de comportamento e não identidades individuais.   
Normalização Min-Max (fit_transform): Os algoritmos de aprendizado supervisionado não compreendem a natureza qualitativa dos dados; eles interpretam apenas a magnitude numérica pura. Sem o escalonamento Min-Max, variáveis com valores numéricos elevados (como tempo de tela em segundos ou salário) dominam indevidamente variáveis de menor valor absoluto (como idade ou número de cliques). A função fit_transform ajusta todos os atributos para uma mesma escala padronizada entre $0.0$ e $1.0$, permitindo que o algoritmo atribua pesos estatísticos corretos a cada variável.   
