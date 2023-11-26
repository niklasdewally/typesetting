# Note on LaTeX installations

If you do not have a working LaTeX installation, or your installation is not
working with Quarto (it errors on render), you can instead install and use
Quarto's internal version of LaTeX, `TinyTeX`.

```
quarto install tool tinytex
```

`TinyTeX` is only ~100MB, and has a minimal set of packages Quarto needs to
render Markdown to LaTeX. If you are running Quarto's built-in `TinyTeX`, or
`TexLive` it should automatically install missing packages for you on build.

See [Quarto Manual - PDF Engines](https://quarto.org/docs/output-formats/pdf-engine.html).
## St Andrews Lab Machines

**Although lab machines have `TeXLive`, this does not seem to work with Quarto.
Use `TinyTeX`.**

Quarto tries to install missing packages for you, but then cannot find said
packages. Everything works as expected with `TinyTex`.

<!-- vim: cc=80 tw=80
-->
