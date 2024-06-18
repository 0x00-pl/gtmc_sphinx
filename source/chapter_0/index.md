前言
===

语法示例
----

Hallo world!

```{note}
An admonition note!
```

Markdown-friendly directives

:::{note}
This text is **standard** *Markdown*
:::

````{note}
The next info should be nested
```{warning}
Here's my warning
```
````

````{note}
The warning block will be properly-parsed

   ```{warning}
   Here's my warning
   ```

But the next block will be parsed as raw text

    ```{warning}
    Here's my raw text warning that isn't parsed...
    ```
````

``````text
``` {directivename} arguments
:key1: val1
:key2: val2

This is
directive content
```
``````

equal to following in `.rst` file.

```text
.. directivename:: arguments
   :key1: val1
   :key2: val2

   This is
   directive content
```

## cross-reference

(heading-target)=
### Heading

{#paragraph-target}
This is a paragraph, with an `id` attribute.
enabled by `myst_enable_extensions = [..., "attrs_block"]` in `conf.py`.

This is a [span with an `id` attribute]{#span-target} .
enabled by `myst_enable_extensions = [..., "attrs_inline"]` in `conf.py`.

:::{note}
:name: directive-target

This is a directive with a `name` option
:::

[reference1](#heading-target), [reference2](#paragraph-target),
[reference3](#span-target), [reference4](#directive-target)

## Code

```python
from random import randint
print(f"{randint(0, 10)=}")
```

## Definition list

term
: definition

## Math
Since Pythagoras, we know that {math}`a^2 + b^2 = c^2`

$$\pi = 3.14159$$

$\pi = 3.14159$

## LaTeX Math
\begin{gather*}
a_1=b_1+c_1\\
a_2=b_2+c_2-d_2+e_2
\end{gather*}

\begin{align}
a_{11}& =b_{11}&
  a_{12}& =b_{12}\\
a_{21}& =b_{21}&
  a_{22}& =b_{22}+c_{22}
\end{align}

- A list
- \begin{gather*}
  a_1=b_1+c_1\\a_2=b_2+c_2-d_2+e_2
  \end{gather*}

> A block quote
> \begin{gather*}
  a_1=b_1+c_1\\a_2=b_2+c_2-d_2+e_2
  \end{gather*}
 

## Figures

```{figure} https://via.placeholder.com/150
:width: 100px
:align: center

Figure caption
```

## Tables

```{list-table}
:header-rows: 1
:align: center

* - Header 1
  - Header 2
* - Item 1 a
  - Item 2 a
* - Item 1 b
  - Item 2 b
```

## MyST only roles
{sub-ref}`today` | {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read


