# 01_ブール算術

## 概要

- 数を表現し、算術演算を行うための論理ゲートを作成する
- 最終的にALU（算術論理演算器, Arithmetic Logic Unit）を作成する

## 実行環境

- 上記サポートサイトにて説明されている、以下のウェブベースの実行環境にて実行
	- [Nand to Tetris Online IDE](https://nand2tetris.github.io/web-ide)

## メモ
### 数値表現
- 2新数で数値が表現
- 最上位ビットが0の場合は正、負の場合は1であり、負の数は以下の歩数表現で表す
```math
\overline{x} = \begin{cases}
    2^n - x & (x \ne 0) \\
    0 & (x = 0)
  \end{cases}
```

- 表現可能な数値は、以下の範囲となる
```math
-2^{n-1} \leq x \leq 2^{n-1} - 1

```