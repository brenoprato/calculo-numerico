# Atividade Prática III — Métodos Numéricos

## Propósito

Material acadêmico executável para comparar bisseção, Newton e secante nas quatro funções do enunciado, incluindo a tabela das 12 execuções e três animações GIF.

Alunos: Guilherme Bento Ramos (185226) e Breno Porto Pinheiro do Prado (185196).

## Mapa de arquivos

| Arquivo | Papel |
| --- | --- |
| `atividade_3_metodos_numericos.ipynb` | Notebook Colab com implementações, testes, tabela, análise e células que geram/exibem os GIFs. |
| `animacao_bissecao_f1.gif` | Animação gerada do intervalo da bisseção para `f1`. |
| `animacao_newton_f2.gif` | Animação gerada das tangentes de Newton para `f2`. |
| `animacao_secante_f3.gif` | Animação gerada das secantes para `f3`. |
| `requirements.txt` | Dependências mínimas para execução local do notebook. |

## Execução e comportamento

Abra `atividade_3_metodos_numericos.ipynb` no Colab ou execute-o com um kernel Python 3 após instalar `pip install -r requirements.txt`. Execute todas as células em ordem. O notebook usa tolerância `1e-6`, no máximo 100 iterações e retorna histórico, estado de convergência e motivo de falha para cada método. A célula final de animações recria os três GIFs no diretório atual.

Os métodos detectam intervalo sem troca de sinal (bisseção), derivada próxima de zero (Newton), denominador próximo de zero (secante), valores não finitos e limite de iterações. A convergência só é declarada quando o resíduo é menor que a tolerância; tamanho de passo pequeno não basta. Não há serviços externos nem dados persistentes.
