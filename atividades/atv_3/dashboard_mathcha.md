# Roteiro e Conteúdo Pronto para o Dashboard no Mathcha (https://www.mathcha.io/)

Este arquivo contém toda a estrutura, textos, equações em LaTeX e tabelas já formatadas para você montar o dashboard no Mathcha em poucos minutos.

---

## Como montar no Mathcha (Passo a Passo)

1. Acesse [https://www.mathcha.io/editor](https://www.mathcha.io/editor) (faça login ou use online).
2. Crie um novo documento.
3. Copie e cole os blocos de texto e equações abaixo.
4. Para as imagens: clique no botão de **Image** (ou simplesmente arraste os arquivos `.gif` que já estão salvos nesta mesma pasta `atv_3/` para dentro do editor do Mathcha).
5. Ao finalizar, clique em **Share** -> **Publish / Get Shareable Link** para gerar o link do seu dashboard de entrega!

---

# [CONTEÚDO PARA COPIAR E COLAR NO MATHCHA]

### Título:
# Atividade Prática III: Zeros de Funções Reais
**Disciplina:** Cálculo Numérico | **Docente:** Profª. Raquel J. Lobosco  
**Universidade Federal de São Paulo (UNIFESP)**  
**Estudante:** Breno Prato

---

### 1. Link para o Notebook no Google Colab
Link de execução completa com código-fonte, testes e funções comentadas:  
👉 **Google Colab Notebook:**  
`https://colab.research.google.com/github/brenoprato/calculo-numerico/blob/main/atividades/atv_3/resolucao.ipynb`

*(No Mathcha, você pode inserir como Link clicável ou colar o endereço acima).*

---

### 2. Tabela de Resultados Comparativos

*(No Mathcha, você pode usar a ferramenta de Tabela ou colar o bloco LaTeX abaixo usando o modo de fórmula)*

| Função | Método | Valores Iniciais | Raiz Aproximada | $|f(x)|$ Final | Iterações / Status |
| :--- | :---: | :---: | :---: | :---: | :---: |
| $f_1(x) = x^2 - 2$ | **Bisseção** | $[1.0, 2.0]$ | $1.41421356$ | $1.62 \times 10^{-6}$ | 20 (Convergência) |
| $f_1(x) = x^2 - 2$ | **Newton** | $x_0 = 1.5$ | $1.41421356$ | $4.51 \times 10^{-12}$ | 3 (Convergência) |
| $f_1(x) = x^2 - 2$ | **Secante** | $(1.0, 2.0)$ | $1.41421356$ | $8.93 \times 10^{-10}$ | 5 (Convergência) |
| $f_2(x) = x^3 - x - 2$ | **Bisseção** | $[1.0, 2.0]$ | $1.52137971$ | $4.27 \times 10^{-6}$ | 20 (Convergência) |
| $f_2(x) = x^3 - x - 2$ | **Newton** | $x_0 = 1.5$ | $1.52137971$ | $5.89 \times 10^{-7}$ | 2 (Convergência) |
| $f_2(x) = x^3 - x - 2$ | **Secante** | $(1.0, 2.0)$ | $1.52137971$ | $7.02 \times 10^{-9}$ | 6 (Convergência) |
| $f_3(x) = e^{-x} - x$ | **Bisseção** | $[0.0, 1.0]$ | $0.56714320$ | $2.35 \times 10^{-7}$ | 20 (Convergência) |
| $f_3(x) = e^{-x} - x$ | **Newton** | $x_0 = 0.5$ | $0.56714329$ | $1.96 \times 10^{-7}$ | 2 (Convergência) |
| $f_3(x) = e^{-x} - x$ | **Secante** | $(0.0, 1.0)$ | $0.56714329$ | $2.54 \times 10^{-8}$ | 4 (Convergência) |
| $f_4(x) = x^3 - 2x + 2$ | **Bisseção** | $[-2.0, -1.0]$ | $-1.76929235$ | $3.52 \times 10^{-6}$ | 20 (Convergência) |
| $f_4(x) = x^3 - 2x + 2$ | **Newton** | $x_0 = -2.0$ | $-1.76929235$ | $5.05 \times 10^{-13}$ | 4 (Convergência) |
| $f_4(x) = x^3 - 2x + 2$ | **Secante** | $(-2.0, -1.0)$ | $-1.76929235$ | $5.59 \times 10^{-7}$ | 6 (Convergência) |

---

### 3. Animações Gráficas do Processo de Aproximação

*(No Mathcha: arraste para cá os 3 arquivos .gif gerados pelo notebook)*

#### 3.1 Método da Bisseção em $f_2(x) = x^3 - x - 2$ (Intervalo $[1, 2]$)
*(Inserir aqui: `animacao_bissecao.gif`)*  
- **Descrição geométrica:** A animação ilustra a divisão binária contínua do intervalo. A cada iteração, calcula-se o ponto médio $m_k = \frac{a_k + b_k}{2}$ e descarta-se o subintervalo que não preserva a mudança de sinal ($f(a) \cdot f(b) < 0$). O intervalo se contrai deterministicamente por um fator de $\frac{1}{2}$ por passo, garantindo convergência incondicional em 20 passos para a tolerância de $10^{-6}$.

#### 3.2 Método de Newton-Raphson em $f_1(x) = x^2 - 2$ ($x_0 = 2.0$)
*(Inserir aqui: `animacao_newton.gif`)*  
- **Descrição geométrica:** A animação exibe a aproximação da curva pela reta tangente no ponto $(x_k, f(x_k))$, cuja equação é $y = f(x_k) + f'(x_k)(x - x_k)$. A interseção da reta tangente com o eixo das abscissas define a nova aproximação $x_{k+1} = x_k - \frac{f(x_k)}{f'(x_k)}$. Observa-se a convergência quadrática ($p = 2$), onde a raiz $\sqrt{2} \approx 1.41421356$ é encontrada com altíssima exatidão em apenas 3 iterações.

#### 3.3 Método da Secante em $f_4(x) = x^3 - 2x + 2$ ($(x_0, x_1) = (-2, -1)$)
*(Inserir aqui: `animacao_secante.gif`)*  
- **Descrição geométrica:** A animação demonstra a interpolação linear utilizando os dois últimos pontos $(x_{k-1}, f(x_{k-1}))$ e $(x_k, f(x_k))$. A reta secante que une esses pontos cruza o eixo $y=0$ no ponto $x_{k+1}$. Esse método alcança taxa superlinear de convergência ($p \approx 1.618$) sem a necessidade de avaliar a derivada analítica $f'(x)$.

---

### 4. Síntese Teórica e Conclusões

1. **Taxas e Ordens de Convergência:**
   - **Bisseção (Linear, $p = 1$):** O erro satisfaz $e_{k+1} \approx \frac{1}{2}e_k$. Sua grande virtude é a robustez absoluta sob o Teorema de Bolzano, sendo insensível à não-linearidade local da função.
   - **Secante (Superlinear, $p \approx 1.618$):** Aproxima a derivada por diferenças finitas. É muito rápida e requer apenas **1 avaliação de função por passo** (reaproveitando o valor anterior).
   - **Newton-Raphson (Quadrática, $p = 2$):** O erro satisfaz $e_{k+1} \approx C e_k^2$, dobrando o número de algarismos significativos a cada iteração próximo da raiz. Exige $f(x)$ e $f'(x)$ a cada iteração.

2. **Critérios de Parada e Detecção de Falhas:**
   - Foi adotado um critério composto: parada quando $|f(x)| < 10^{-6}$ ou quando a variação espacial $|x_{k+1} - x_k| < 10^{-6}$.
   - O algoritmo trata e interrompe com segurança casos degenerados: ausência de troca de sinal inicial ($f(a)f(b) > 0$), derivada nula ($f'(x) \approx 0$) e divisão por zero na secante ($f(x_k) \approx f(x_{k-1})$).
