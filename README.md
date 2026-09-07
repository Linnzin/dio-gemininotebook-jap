# 📓 dio-gemininotebook-jap

Entrega do desafio **"Lab Project"** do Bootcamp Bradesco - GenAI, Dados & Cyber da plataforma [DIO](https://www.dio.me/).

Este repositório reúne um **Gemini Notebook** configurado para auxiliar nos estudos da **Língua Japonesa**, alimentado com fontes confiáveis de gramática, kanji e vocabulário — permitindo respostas contextualizadas e fiéis ao material de referência, em vez de depender apenas do conhecimento genérico do modelo.

---

## 📑 Sumário

- [Estrutura do Repositório](#-estrutura-do-repositório)
- [Configuração do Gemini Notebook](#-configuração-do-gemini-notebook)
- [Fontes de Informação](#-fontes-de-informação)
- [Prompts](#-prompts)
- [Exemplo de Saída](#-exemplo-de-saída)
- [Licença](#-licença)

---

## 📂 Estrutura do Repositório

```
dio-gemininotebook-jap
├── docs                                  // Fontes usadas no Notebook
│   └── guide_links                       // Links de guias online transcritos
│       ├── tae_kims_guide_links.md
│       └── tofugu_japanese_grammar_links.md
│   ├── full_tae_kims_guide.txt           // Guia de Tae Kim compactado (transcrição completa)
│   └── full_tofugu_japanese_grammar.txt  // Artigos da Tofugu compactados
├── prompts                               // Prompts reutilizáveis e system prompt
│   ├── resultados_esperados              // Resultados esperados dos prompts reutilizáveis
│   │   └── resultado_escolher_assunto.md
│   ├── prompt_escolher_assunto.md
│   └── system_prompt.md
├── .gitignore
├── LICENSE                                // Creative Commons BY-NC-SA 4.0
├── mapa_mental_exemplo.png
└── README.md                              // Este arquivo!
```

> ℹ️ Materiais protegidos por direitos autorais (como o livro de Heisig e o guia de Tae Kim em PDF) são usados apenas como referência local durante a montagem do Notebook e **não são versionados** neste repositório — por isso não aparecem na árvore acima.

---

## ⚙️ Configuração do Gemini Notebook

| Configuração | Valor |
|---|---|
| **Estilo de Conversa** | Personalizado → [`system_prompt.md`](/prompts/system_prompt.md) |
| **Tamanho da Resposta** | Mais Longa |

---

## 📚 Fontes de Informação

O plano gratuito do Gemini Notebook permite no máximo 50 fontes. Para contornar esse limite, várias fontes foram condensadas em arquivos de texto (`.txt`) usando um script em Python — o que permitiu incorporar **mais de 300 fontes** ao Notebook. A lista completa dos links utilizados pode ser consultada em [`/docs/guide_links`](/docs/guide_links).

Fontes utilizadas:

* **James W. Heisig** — *Remembering the Kanji* (4ª Edição, Vol. 1)
  > Utilizado apenas como referência teórica. O material não é disponibilizado neste repositório por estar protegido por direitos autorais.

* **Tae Kim** — *Japanese Grammar Guide* (Livro, 2012)
  > Obra publicada por **Tae Kim** e licenciada sob [Creative Commons CC BY-NC-SA 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/). Fonte original: [Guide to Japanese](http://www.guidetojapanese.org/).

* **Tae Kim** — *Tae Kim's Guide to Japanese Grammar* (Transcrição Web)
  > Conteúdo original por **Tae Kim** ([Tae Kim's Guide to Learning Japanese](http://www.guidetojapanese.org/learn/)), obtido via [Open of Course](https://www.open-of-course.org/courses/file.php/62/index.html#contents) e licenciado sob [CC BY-NC-SA 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/). O guia foi transcrito e disponibilizado neste repositório em [`full_tae_kims_guide.txt`](/docs/full_tae_kims_guide.txt).

* **Tofugu** — *Japanese Grammar Guides*
  > Utilizado apenas como referência teórica. A transcrição não é disponibilizada neste repositório por possuir todos os direitos reservados à Tofugu LLC.

* **Tofugu** — [*Learn Japanese: A Ridiculously Detailed Guide*](https://www.tofugu.com/learn-japanese/)

* **Doki Doki Japan** — [*Japanese Levels: Complete Guide to Understanding the JLPT*](https://dokidokijapan.com/en/blog/japanese-levels-what-each-one-means-and-what-is-expected-of-you/)

---

## 💬 Prompts

Prompts prontos para uso no Notebook.

* **[`system_prompt.md`](/prompts/system_prompt.md)**
  > Prompt de sistema. Deve ser usado nas configurações do Notebook — dita como a IA deve se comportar.

* **[`prompt_escolher_assunto.md`](/prompts/prompt_escolher_assunto.md)**
  > Prompt de chat, usado quando é necessário escolher um novo assunto para estudar. **Lembre-se de adaptar o contexto antes de usar!**

### Resultados Esperados

Os resultados esperados de cada prompt ficam armazenados em [`/prompts/resultados_esperados/`](/prompts/resultados_esperados/), permitindo comparar a saída obtida com o comportamento previsto.

---

## 🖼️ Exemplo de Saída

![Mapa mental: Formas de estudo](/mapa_mental_exemplo.png)

---

## 📄 Licença

Este projeto está licenciado sob [Creative Commons BY-NC-SA 4.0](/LICENSE). Consulte o arquivo [`LICENSE`](/LICENSE) para mais detalhes, e as notas de cada fonte acima para as licenças específicas do material de terceiros.