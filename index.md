---
author-meta:
  - Wesley Yarde
date-meta: July 1, 2021
pagetitle: Gino Keva in under 5 minutes
url-gh: https://github.com/wyarde
url-gino-keva: https://github.com/philips-software/gino-keva
url-talk: https://wyarde.github.io/talk-gino-keva-in-under-5-minutes
x: '<span style="color:White">**'
xx: "**</span>"
---

## $pagetitle$

\
The Gathering\
$date-meta$\

## \

:::: {.r-stack style="font-size:var(--heading2-size); color:gray"}

[$x$Gino Keva$xx$]{.fragment .fade-out data-fragment-index="1"}

[A $x$Gino Keva$xx$]{.fragment .fade-in-then-out data-fragment-index="1"}

[A $x$Gi$xx$t $x$no Keva$xx$]{.fragment .fade-in-then-out data-fragment-index="2"}

[A $x$Gi$xx$t $x$no$xx$tes $x$Keva$xx$]{.fragment .fade-in-then-out data-fragment-index="3"}

[A $x$Gi$xx$t $x$no$xx$tes $x$Ke$xx$y $x$va$xx$]{.fragment .fade-in-then-out data-fragment-index="4"}

[A $x$Gi$xx$t $x$no$xx$tes $x$Ke$xx$y $x$va$xx$lue]{.fragment .fade-in-then-out data-fragment-index="5"}

[A $x$Gi$xx$t $x$no$xx$tes $x$Ke$xx$y $x$va$xx$lue store]{.fragment .fade-in-then-out data-fragment-index="6"}

::::

## Git Notes

<sub><sup>_Supplement a commit message without changing the commit itself_</sup></sub>

- <span style="color:Moccasin">`git notes add|remove|show|list`</span>
- Stored as commits in refs/notes/

## Gino Keva

<sub><sup>_A Git notes key value store_</sup></sub>

- <span style="color:Moccasin">`gino-keva set|unset|get|list`</span>
- Gino Keva operates on the current commit
- If no note is available, nearest one is copied over

### Example syntax

```console
$$ gino-keva set foo bar
$$ gino-keva get foo
bar
```

:::{.element: class="fragment" data-fragment-index="1"}

```console
$$ gino-keva set counter 12 && gino-keva list
COUNTER=12
FOO=bar
```

:::

:::{.element: class="fragment" data-fragment-index="2"}

```console
$$ git commit --allow-empty -m empty
$$ gino-keva set counter 13 && gino-keva list
COUNTER=13
FOO=bar
```

:::

## A build pipeline

![New feature, build 46](images/pipeline.png)

### Gino Keva through history

![](images/git_history.png)

# End

|                    Gino Keva                    |               This talk               |
| :---------------------------------------------: | :-----------------------------------: |
| [![](images/qr_gino-keva.png)]($url-gino-keva$) | [![](images/qr_talk.png)]($url-talk$) |
