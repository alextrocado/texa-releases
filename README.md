# TEXA

**O processador de texto que fala LaTeX.** Escreve como no Word e obtém LaTeX limpo. Ou abre um
`.tex` e edita-o como um documento normal. Funciona em macOS (Apple silicon) e Windows.

[⬇ Descarregar a versão mais recente](https://github.com/alextrocado/texa-releases/releases/latest)

- **macOS:** abre o `.dmg` e arrasta o TEXA para Aplicações.
- **Windows:** corre o `setup.exe`.

Depois de instalado, o TEXA procura versões novas quando o abres e pergunta se queres atualizar.

---

## Exemplos de utilização

### 1. Do Word para LaTeX

1. Abre um `.docx` (Ficheiro › Abrir, ou arrasta-o para a janela).
2. No separador **LaTeX**, carrega em **Painel LaTeX**: o código LaTeX do documento aparece ao lado
   da página.
3. Carrega em **Compilar**: o PDF abre feito pelo LaTeX.
4. **Guardar como** › `.tex` grava o ficheiro LaTeX (as imagens ficam ao lado, `nome-1.png`…).

Os títulos passam a `\section`, as listas a `itemize`/`enumerate`, as tabelas a `tabular`, as notas
a `\footnote`, as citações a `\cite` com `thebibliography`, as legendas a `\caption` com `\label`
e `\ref`.

### 2. Do LaTeX para Word

1. Abre um `.tex`: o TEXA mostra-o como um documento normal, com as equações desenhadas.
2. Edita o texto, as tabelas e as equações como no Word.
3. Grava em `.tex` outra vez, ou em `.docx` para enviar a quem usa Word.

Por exemplo, este ficheiro:

```latex
\documentclass[12pt,a4paper]{article}
\usepackage[portuguese]{babel}
\title{Funções reais}
\author{Prof. Silva}
\begin{document}
\maketitle
\section{Domínio}
O domínio de $f(x)=\sqrt{x-2}$ é $[2,+\infty[$.
\begin{equation}
  f'(x)=\frac{1}{2\sqrt{x-2}}
\end{equation}
\end{document}
```

abre com o título, a secção e as duas equações editáveis. Gravado outra vez em LaTeX, mantém a
classe, as opções, `\maketitle` e a equação numerada.

### 3. Equações com o teclado (atalhos do MathType)

| Teclas (macOS) | Faz |
|---|---|
| Cmd+E | Nova equação |
| Cmd+Shift+E | Equação no meio do texto |
| Ctrl+F | Fração |
| Ctrl+H / Ctrl+L | Expoente / índice |
| Ctrl+R | Raiz quadrada |
| Ctrl+G, depois p | π (Ctrl+G e uma letra: letra grega) |
| Ctrl+D, depois R | ℝ |
| Ctrl+I | Integral |
| Tab | Casa seguinte do modelo |

No Windows, Cmd é Ctrl. Todos os atalhos estão em **Inserir › Atalhos de Equações** e podem ser
mudados: clica com o botão direito num símbolo da Paleta de Equações › **Definir Atalho…**.

Também podes escrever `$x^2+1$` no texto: com a opção **Escrever $…$ para equações** ligada (separador
LaTeX), passa a uma equação.

### 4. Modelos LaTeX prontos

**LaTeX › Modelos LaTeX** abre 16 modelos em português:

- **Avaliação:** teste (classe `exam`), teste ao estilo do exame nacional, escolha múltipla, mini-teste;
- **Fichas:** ficha de trabalho, ficha com resoluções, ficha (classe `exam`), formulário;
- **Escola:** plano de aula;
- **Académicos:** artigo, relatório, relatório de laboratório, tese, livro;
- **Outros:** carta formal, currículo.

Escolhe um, escreve por cima e compila.

### 5. O aspeto do PDF

No separador **LaTeX**, em **Aspeto**:

- **LaTeX clássico** (por omissão): o PDF tem o aspeto de um documento feito à mão em LaTeX, com a
  letra Computer Modern, secções numeradas e `\maketitle`;
- **Igual ao ecrã**: o PDF imita a página do documento (letra, margens, cores e espaçamentos).

### 6. PDF para documento editável

Arrasta um PDF para a janela: o texto, os títulos e as imagens passam a um documento que podes
editar e gravar em `.docx` ou `.tex`.

---

## Para compilar LaTeX

O TEXA escreve e lê LaTeX sem nada instalado. Para **Compilar** (fazer o PDF) é preciso uma
distribuição de TeX:

- **macOS:** [MacTeX](https://www.tug.org/mactex/)
- **Windows:** [MiKTeX](https://miktex.org/) ou [TeX Live](https://www.tug.org/texlive/)

Se não estiver instalada, o TEXA diz-te isso e mostra a ligação para a descarregares.

## Línguas

A interface está em 20 línguas, entre elas português, inglês, espanhol, francês e alemão. Muda-se
em Ficheiro › Opções.

---

© 2026 Alexandre Trocado · mail@alexandretrocado.com
