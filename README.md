
# Analisando-Dados-com-Pandas-SQL.


import pandas as pd

df = pd.read_csv('pasta/arquivo.csv', sep = 'oque separa o df')

### Criando uma coluna

df['new'] = df['W'] + df['Y']

### Removendo uma coluna

df.drop('new',axis=1,inplace=True)

### Selecionando Linhas

df.loc['A']

### Ou selecionando com base na posição ao invés de rótulo

df.iloc[2]

# Redefinindo o index

### Redefinir para o padrão 0,1 .... n índice

df.reset_index()

novoind = 'CA NY WY OR CO'.split()

df['Estados'] = novoind

### Setando o index
df.set_index('Estados', inplace=True)
