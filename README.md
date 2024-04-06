# analise_dataset_acidentes_gen_ai
analise_dataset_acidentes_gen_ai

Gostaria de compartilhar com vocês o resultado de minha primeira experiência com IA Generativa.

Utilizei a API da OpenAI juntamente com o dataset de acidentes de transito reportados pelo DPRF para realizar análises exploratórias de acidentes que ocorreram no Piauí no corrente ano.

O passo-a-passo do desenvolvimento foi o seguinte:
1 - Definição das colunas relevantes do Dataset;
2 - Combinar/concatenar as colunas relevantes em uma nova coluna;
3 - Adicionar a coluna "embedding" (que é uma representação numérica de palavras ou frases que captura informações semânticas sobre o seu significado) ao DF;
4 - Salvar o Dataframe com os "embedding" (ideal para reduzir custos com a API)
5 - Acessar o DF salvo;
6 - Definir a pergunta que será realizada;
7 - Utilizar a similaridade de cosseno para definir a similaridade entre a pergunta e cada linha do DF;
8 - Definir a quantidade de linhas mais similares a pergunta a serem retornadas;
9 - Utilizar a saída das linhas mais similares como input para o Modelo de geração de textos;

E o resultado é o seguinte:
PS: como entusiasta no assunto, o resultado foi satisfatório, apesar de ainda estar buscando melhores metodologias.
