+++
title = "This one uses the awesome power of Org"
author = ["Alain Picard"]
date = 2020-08-01T00:00:00+10:00
draft = true
math = true
+++

The question is: _who_ is doing the exporting?  I think
it's `org-hugo-auto-export-mode` in the _Local Variables_.

\\( e^{i\pi} + 1 = 0 \\)

-   Here we refer to [Blog](/blog)
-   And make a change
-   Here we refer to

<a src="/">The home page</a>

-   And here to an inner link on [the foo page](/blog/foo)
-   And highlighting is still failing.

```clojure
(defn foo
  "Do some foo"
  [x y]
  (log "Some foobar message")
  (+ x y))
```

<!--more-->

{{< highlight lisp "hl_lines=2 -n 20" >}}
(message "This is line 1")
(message "This is line 2")
(message "This is line 3")
{{< /highlight >}}


## Equations: {#equations}

LaTeX formatted equation: \\( E = -J \sum\_{i=1}^N s\_i s\_{i+1} \\)


## Another one {#another-one}

\begin{equation}
\label{eq:1}
C = W\log\_{2} (1+\mathrm{SNR})
\end{equation}

And that's _all_, folks!


## Weight {#weight}

<div class="ox-hugo-table striped--light-gray">
<div></div>

| Date                                                                                               | Weight (kg) | Notes                   |
|----------------------------------------------------------------------------------------------------|-------------|-------------------------|
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2009-10-14 Wed&gt;</span></span>       | 72.4        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2009-10-15 Thu&gt;</span></span>       | 72.6        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2009-10-17 Sat&gt;</span></span>       | 72.8        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2009-10-18 Sun&gt;</span></span>       | 72.8        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2009-10-19 Mon&gt;</span></span>       | 73.4        | (!!)                    |
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2009-10-20 Tue&gt;</span></span>       | 73.2        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2009-10-21 Wed&gt;</span></span>       | 72.8        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2010-04-04 Sun&gt;</span></span>       | 71.4        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">[2013-02-05 Tue]</span></span>             | 73.0        | Weight Watchers, reboot |
| <span class="timestamp-wrapper"><span class="timestamp">[2013-02-06 Wed]</span></span>             | 72.8        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">[2013-02-07 Thu]</span></span>             | 74.0        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">[2013-02-14 Thu]</span></span>             | 74.4        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">[2013-07-03 Wed]</span></span>             | 72.4        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">[2013-12-28 Sat]</span></span>             | 74.2        | Ouch.                   |
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2016-01-06 Wed 17:33&gt;</span></span> | 75.6        |                         |
| <span class="timestamp-wrapper"><span class="timestamp">&lt;2017-08-29 Tue 09:14&gt;</span></span> | 77.0        | Ouch!!                  |

</div>


## Inline styled table {#inline-styled-table}

<style>
.my-table th,
.my-table td {
    padding: 20px;
    text-align: left;
}
</style>

<div class="ox-hugo-table my-table">
<div></div>

<div class="table-caption">
  <span class="table-number">Table 1</span>:
  Table with verbatim CSS
</div>

| h1  | h2  | h3  |
|-----|-----|-----|
| abc | def | ghi |

</div>
