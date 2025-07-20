
# 📚 Anotações de Estudo: Negrito e Itálico em HTML

📅 Criado em: **20 de julho de 2025**  
📚 Matéria:**Programação Web (HTML5 e CSS3)**  
✍️ Autor: **Marco**

## 1. Introdução: Semântica vs. Apresentação

Essa aula mostra como o mesmo visual (negrito/itálico) pode ter significados diferentes em HTML. A chave aqui é separar **semântica** de **estilo visual**.

- **HTML:** cuida do _significado_ do conteúdo.
- **CSS:** cuida da _aparência_ do conteúdo.

Quando falamos de negrito e itálico, o HTML tem tags diferentes com propósitos diferentes, mesmo que o navegador mostre do mesmo jeito.

---

## 2. Negrito em HTML: `<b>` vs. `<strong>`

### 🔸 `<b>` (Negrito visual, sem significado)

- **Propósito:** só muda o visual, sem dar importância ao conteúdo.
- **Usar quando:** quer destacar algo, mas sem dizer que é mais importante que o resto.

#### Exemplo:
```html
<p>Apenas um <b>nome</b> para destaque visual.</p>
<p>Clique no botão <b>Salvar</b> para continuar.</p>
```

- **Semântica:** nenhuma.

---

### 🔹 `<strong>` (Negrito com importância)

- **Propósito:** mostra que aquele texto tem peso, importância ou urgência.
- **Usar quando:** for algo que precisa de destaque **pelo significado**.

#### Exemplo:
```html
<p>Este é um aviso muito <strong>importante</strong> para a sua segurança.</p>
<p>Lembre-se: <strong>nunca compartilhe sua senha</strong> com ninguém.</p>
```

- **Semântica:** sim. Leitores de tela até mudam o tom da fala!

✅ **Regra de Ouro:**  
Se for só visual, use `<b>`.  
Se for importante mesmo, use `<strong>`.

---

## 3. Itálico em HTML: `<i>` vs. `<em>`

### 🔸 `<i>` (Itálico visual, sem ênfase)

- **Propósito:** muda o estilo, mas não muda o sentido.
- **Usar quando:** palavras em outro idioma, nomes de livros, pensamentos internos etc.

#### Exemplo:
```html
<p>A palavra <i>status</i> vem do latim.</p>
<p>O livro favorito dela é <i>Cem Anos de Solidão</i>.</p>
```

- **Semântica:** nenhuma.

---

### 🔹 `<em>` (Ênfase semântica)

- **Propósito:** dá ênfase **que muda o sentido da frase**.
- **Usar quando:** você quer que a palavra receba destaque de verdade.

#### Exemplo:
```html
<p>Eu <em>amo</em> chocolate.</p> <!-- Ênfase no verbo -->
<p>Eu amo <em>chocolate</em>.</p> <!-- Ênfase no objeto -->
```

- **Semântica:** sim. Leitores de tela também destacam isso.

✅ **Regra de Ouro:**  
Se for só estilo, use `<i>`.  
Se for mudar o tom ou sentido, use `<em>`.

---

## 4. Impacto e Boas Práticas

- **Acessibilidade:** `<strong>` e `<em>` são entendidos por leitores de tela. `<b>` e `<i>` não são.
- **SEO:** usar as tags corretas ajuda o Google a entender melhor o conteúdo.
- **Estilo puro? Vai de CSS!**

### Exemplo com CSS:

```html
<span style="font-weight: bold;">texto</span>
<!-- ou melhor ainda com classe -->
<span class="destaque-visual">texto</span>
```

```html
<span style="font-style: italic;">texto</span>
<span class="inclinado">texto</span>
```

---

## 🎯 Conclusão

A escolha entre `<b>/<strong>` e `<i>/<em>` **faz diferença**. Use com consciência:

- Pra destacar visualmente? Use `<b>` e `<i>`.
- Pra dar **significado** e ajudar na **acessibilidade**? Use `<strong>` e `<em>`.

**Quanto mais semântico for seu HTML, melhor para todo mundo — inclusive pra você no futuro!** 😉
