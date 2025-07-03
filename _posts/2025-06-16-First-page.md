---
layout: post
title: 첫 글
description: >
  제 첫번째 글입니다 한글이 잘 써지는지 봐볼까요? 이 글은 연습 글입니다.
tags: [math]
slug : math
math: true
---

그냥 글은 이렇게 쓰면 되네요.
**중요한 것** _기울어지게_ ~~안녕하신가요~~

이런 식으로 여백도 생기네요

# 주제1

이렇게 섹션을 나눌 수도 있습니다

## 주제2 

> 이런 식으로 느낌있게 쓸 수도 있네요
> 네네
> 음음
> 강조하기.

### 주제3

어떤 사실들을 나열할 때는
* hello
* hi
* 안녕


이런 식으로 쓰거나 

1. hi
2. hello
3. 안녕

이런 식으로 쓰면 되네요.

줄 긋기
* * *

# 설명할때

Name
: 김상훈

Born
: 2005

Birthplace
: South Korea

'''
마지막 기능까지 확인
'''

### 사라지는 글씨?

사라져보겠습니다.
{:.faded}

### Latex 수식 연습

어제 힘들게 풀었던 프리드버그 2.2.17 문제의 풀이로 수식 입력을 연습해보겠습니다.

**Problem 2.2.17**  

Let $V$ and $W$ be vector spaces such that $\dim(V) = \dim(W)$, 
and let $T : V \to W$ be linear. Show that there exist ordered bases $\beta$ and $\gamma$ for V and W, respectively, such that $[T]_{\beta}^{\gamma}$ is a diagonal matrix.


**Solution**

Let $\alpha_1 = \{w_1, \ldots, w_k\}$ and $\alpha_2 = \{v_{k+1}, \ldots, v_n\}$ be bases for $R(T)$ and $N(T)$, respectively.

Then, the set $\{v_1, \ldots, v_k \mid v_i \in V, \text{ such that } T v_i = w_i\}$ is linearly independent since $\alpha_1$ is linearly independent.

Thus, $\beta = \{v_1, \ldots, v_k, v_{k+1}, \ldots, v_n\}$ becomes a basis for $V$.

We can show its linear independence:

$$
\begin{array}{l}
c_1 v_1 + \cdots + c_n v_n = 0 \\
\Rightarrow \sum_{i=1}^n c_i T(v_i) = 0 \\
\Rightarrow c_1 w_1 + \cdots + c_k w_k = 0 \\
\Rightarrow c_1 = \cdots = c_k = 0 \\
\Rightarrow c_{k+1} v_{k+1} + \cdots + c_n v_n = 0 \\
\Rightarrow c_{k+1} = \cdots = c_n = 0
\end{array}
$$

Now, by the Replacement Theorem, there exists a set $U = \{w_{k+1}, \ldots, w_n\}$ such that $U \cup \alpha_1$ spans $W$.

We can set $\gamma = U \cup \alpha_1$. Then:

$$
[T]_\beta^\gamma = [a_{ij}], \quad
a_{ij} =
\begin{cases}
\delta_{ij} & \text{if } 1 \leq j \leq k \\
0 & \text{if } k+1 \leq j \leq n
\end{cases}
$$

Therefore, $[T]_\beta^\gamma$ is diagonal. $\blacksquare$

