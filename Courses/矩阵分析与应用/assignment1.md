# assignment1
Exercises

4.

## (1)
将矩阵[A|b]转换成简约的行阶梯表达形式$E_{[A|b]}$

$$ 
A = \left(
    \begin{array}{cccc|c}
      1 & 2 & 1 & 2 & 3 \\
      2 & 4 & 1 & 3 & 4 \\
      3 & 6 & 1 & 4 & 5
    \end{array}
\right) 
 ->  \left(
    \begin{array}{cccc|c}
      1 & 2 & 1 & 2 & 3 \\
      0 & 0 & -1 & -1 & -2 \\
      0 & 0 & -2 & -2 & -4
    \end{array}
\right) 

$$

$$
 ->  \left(
    \begin{array}{cccc|c}
      1 & 2 & 1 & 2 & 3 \\
      0 & 0 & 1 & 1 & 2 \\
      0 & 0 & 0 & 0 & 0
    \end{array}
\right) 

$$
$$
 ->  \left(
    \begin{array}{cccc|c}
      1 & 2 & 0 & 1 & 1 \\
      0 & 0 & 1 & 1 & 2 \\
      0 & 0 & 0 & 0 & 0
    \end{array}
\right) 
$$
观察发现最后一列是非基本列，所以有解，可知非齐次系统的通解为

$$
\left(
    \begin{array}{c}
      x_1 \\
      x_2 \\
      x_3 \\
      x_4
    \end{array}
\right) 
= 
\left(
    \begin{array}{c}
      1-2x_2-x_4 \\
      x_2 \\
      2-x_4 \\
      x_4
    \end{array}
\right) 
= \left(
    \begin{array}{c}
      1 \\
      0 \\
      2 \\
      0 
    \end{array}
\right) 
+ x_2\left(
    \begin{array}{c}
      -2 \\
      1 \\
      0 \\
      0 
    \end{array}
\right)
+ x_4\left(
    \begin{array}{c}
      -1 \\
      0 \\
      -1 \\
      1 
    \end{array}
\right)
$$

## (2)

![](_v_images/20190910121433697_7080.png =600x)
