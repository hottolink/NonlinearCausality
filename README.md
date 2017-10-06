# Jupyter Notebook
テックブログで紹介したサンプルコードを実行しながら理解を深めていくためにJupyter Notebookを公開しております。

## 必要な環境の準備
1. Jupyter (iPython Notebook)を導入します。Anaconda等で事前にインストールしてください。
2. Julia 0.5.2のインストール：[https://julialang.org/downloads/oldreleases.html](https://julialang.org/downloads/oldreleases.html)
3. JuliaのREPLを起動し、必要なパッケージをインストールします。上手くいかない場合は各パッケージのGitを参考しましょう。


```
>>julia

========
# この辺のパッケージインストールはREPLで行います。
Pkg.update()
Pkg.status()

Pkg.add("IJulia")           # JupyterにJuliaカーネルを追加 https://github.com/JuliaLang/IJulia.jl
Pkg.add("Distributions")    # 乱数生成や、確率分布を使う時用 https://github.com/JuliaStats/Distributions.jl
Pkg.add("DataFrames")       # RのようなDataFramesを使う時用 https://github.com/JuliaData/DataFrames.jl
Pkg.add("Gadfly")           # グラフ描画用 https://github.com/GiovineItalia/Gadfly.jl
========
```

整いたらJupyterを起動し、TechBlog_NonlinearCausality.ipynbを開いて実験開始します。
