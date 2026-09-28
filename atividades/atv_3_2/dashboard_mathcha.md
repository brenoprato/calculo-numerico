# Atividade Prática III — Métodos Numéricos

**Curso:** Cálculo Numérico  
**Alunos:** Guilherme Bento Ramos (185226) e Breno Porto Pinheiro do Prado (185196)

## Notebook executável

[Abrir a resolução no Google Colab](https://colab.research.google.com/github/brenoprato/calculo-numerico/blob/main/atividades/atv_3_2/resolucao.ipynb)

## Resultados das 12 execuções

| Função | Método | Valores iniciais | Raiz aproximada | \|f(x)\| final | Iterações/resultado |
| --- | --- | --- | ---: | ---: | --- |
| f1(x) = x² − 2 | Bisseção | [1, 2] | 1.4142136574 | 2.687e-07 | 21 — convergiu |
| f1(x) = x² − 2 | Newton | 1.5 | 1.4142135624 | 4.511e-12 | 3 — convergiu |
| f1(x) = x² − 2 | Secante | (1, 2) | 1.4142135621 | 8.931e-10 | 5 — convergiu |
| f2(x) = x³ − x − 2 | Bisseção | [1, 2] | 1.5213797092 | 1.450e-08 | 22 — convergiu |
| f2(x) = x³ − x − 2 | Newton | 1.5 | 1.5213798060 | 5.894e-07 | 2 — convergiu |
| f2(x) = x³ − x − 2 | Secante | (1, 2) | 1.5213797080 | 7.015e-09 | 6 — convergiu |
| f3(x) = exp(−x) − x | Bisseção | [0, 1] | 0.5671434402 | 2.348e-07 | 20 — convergiu |
| f3(x) = exp(−x) − x | Newton | 0.5 | 0.5671431650 | 1.965e-07 | 2 — convergiu |
| f3(x) = exp(−x) − x | Secante | (0, 1) | 0.5671433066 | 2.538e-08 | 4 — convergiu |
| f4(x) = x³ − 2x + 2 | Bisseção | [-2, -1] | -1.7692923546 | 2.551e-09 | 21 — convergiu |
| f4(x) = x³ − 2x + 2 | Newton | -2.0 | -1.7692923542 | 5.054e-13 | 4 — convergiu |
| f4(x) = x³ − 2x + 2 | Secante | (-2, -1) | -1.7692922786 | 5.594e-07 | 6 — convergiu |

## Animações

Faça upload/anexe cada GIF abaixo no Mathcha no respectivo espaço. O editor pode exibir somente uma imagem estática; nesse caso, mantenha também o link clicável para o arquivo GIF no GitHub.

### Bisseção em f1

**Espaço para anexar:** `animacao_bissecao_f1.gif`  
[Abrir GIF no GitHub](https://github.com/brenoprato/calculo-numerico/blob/main/atividades/atv_3_2/animacao_bissecao_f1.gif)  
Mostra `f1(x) = x² − 2`, o intervalo que contém a raiz e sua redução a cada iteração da bisseção.

### Newton em f2

**Espaço para anexar:** `animacao_newton_f2.gif`  
[Abrir GIF no GitHub](https://github.com/brenoprato/calculo-numerico/blob/main/atividades/atv_3_2/animacao_newton_f2.gif)  
Mostra `f2(x) = x³ − x − 2` e as retas tangentes usadas nas iterações de Newton.

### Secante em f3

**Espaço para anexar:** `animacao_secante_f3.gif`  
[Abrir GIF no GitHub](https://github.com/brenoprato/calculo-numerico/blob/main/atividades/atv_3_2/animacao_secante_f3.gif)  
Mostra `f3(x) = exp(−x) − x` e as retas secantes pelos dois pontos usados em cada passo.

## Conclusão

As 12 execuções convergiram com tolerância de `1e-6`. A bisseção foi mais previsível, mas exigiu mais iterações; Newton foi mais rápido com os valores iniciais usados; a secante também convergiu rapidamente sem usar derivada.

## Montagem no Mathcha

1. Crie um novo documento em [Mathcha](https://www.mathcha.io/).
2. Copie e cole este conteúdo; ajuste a tabela se necessário no editor.
3. Insira os três GIFs nos espaços indicados por upload/anexo e mantenha os links do GitHub como alternativa clicável.
4. Confirme que o link do Colab abre `resolucao.ipynb` antes de compartilhar o dashboard.
