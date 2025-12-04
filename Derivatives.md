# The Derivative in Calculus

The derivative is one of the fundamental concepts in calculus, along with the integral. It represents the **rate of change** of a function.

---

## 1. Definition and Interpretation

* **Geometrically:** The derivative of a function $f(x)$ at a point $x=a$ is the **slope of the tangent line** to the graph of $f(x)$ at the point $(a, f(a))$.
    

* **Physically/Conceptually:** The derivative measures the **instantaneous rate of change** of the function's output ($y$ or $f(x)$) with respect to its input ($x$).
    * If $f(t)$ is the **position** of an object, then $f'(t)$ (the derivative) is its **instantaneous velocity**.

---

## 2. Formal Definition (Limit Definition)

The derivative of $f(x)$, denoted $f'(x)$ or $\frac{dy}{dx}$, is formally defined using a limit:

$$f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$

This is the limit of the **average rate of change** (the slope of a secant line) as the interval ($h$) approaches zero, turning it into the **instantaneous rate of change** (the slope of the tangent line).

---

## 3. Key Differentiation Rules

To avoid using the limit definition constantly, we use rules:

| Rule | Function | Derivative ($f'(x)$ or $\frac{dy}{dx}$) |
| :--- | :--- | :--- |
| **Constant Rule** | $f(x) = c$ | $0$ |
| **Power Rule** | $f(x) = x^n$ | $n x^{n-1}$ |
| **Sum/Difference Rule** | $f(x) \pm g(x)$ | $f'(x) \pm g'(x)$ |
| **Product Rule** | $f(x)g(x)$ | $f'(x)g(x) + f(x)g'(x)$ |
| **Quotient Rule** | $\frac{f(x)}{g(x)}$ | $\frac{f'(x)g(x) - f(x)g'(x)}{[g(x)]^2}$ |
| **Chain Rule** | $f(g(x))$ | $f'(g(x)) \cdot g'(x)$ |

---

## 4. Examples with Breakdown

### 4.1. Power Rule and Constant Multiple Rule

**Example:** Find the derivative of the function $f(x) = 5x^3$.

| Step | Breakdown | Rule Used |
| :--- | :--- | :--- |
| **Original Function** | $f(x) = 5x^3$ | |
| **Apply Power Rule** | $\frac{d}{dx} (x^3) = 3x^{3-1} = 3x^2$ | Power Rule: $\frac{d}{dx}(x^n) = nx^{n-1}$ |
| **Apply Constant Multiple Rule** | $f'(x) = 5 \cdot (3x^2)$ | Constant Multiple Rule: $\frac{d}{dx}[c \cdot f(x)] = c \cdot f'(x)$ |
| **Simplify** | $f'(x) = **15x^2**$ | |

---

### 4.2. Sum/Difference Rule

**Example:** Find the derivative of the polynomial $g(x) = 2x^4 - 6x + 7$.

| Step | Breakdown | Rule Used |
| :--- | :--- | :--- |
| **Original Function** | $g(x) = 2x^4 - 6x + 7$ | |
| **Differentiate term by term** | $g'(x) = \frac{d}{dx}(2x^4) - \frac{d}{dx}(6x) + \frac{d}{dx}(7)$ | Sum/Difference Rule |
| **Apply Power/Constant Rules** | $g'(x) = (2 \cdot 4x^{4-1}) - (6 \cdot 1x^{1-1}) + 0$ | Power Rule & Constant Rule |
| **Final Result** | $g'(x) = **8x^3 - 6**$ | |

---

### 4.3. Product Rule

**Example:** Find the derivative of $y = (x^2 + 1)(3x - 5)$.

Let $f(x) = x^2 + 1$ and $g(x) = 3x - 5$.

| Step | Breakdown | Rule Used |
| :--- | :--- | :--- |
| **Find Components** | $f'(x) = 2x$; $g'(x) = 3$ | |
| **Apply Product Rule** | $\frac{dy}{dx} = f'(x)g(x) + f(x)g'(x)$ | Product Rule |
| **Substitute** | $\frac{dy}{dx} = (2x)(3x - 5) + (x^2 + 1)(3)$ | |
| **Simplify** | $\frac{dy}{dx} = (6x^2 - 10x) + (3x^2 + 3)$ | |
| **Final Result** | $\frac{dy}{dx} = **9x^2 - 10x + 3**$ | |

---

### 4.4. Chain Rule (Composite Functions)

**Example:** Find the derivative of $h(x) = (2x + 1)^4$.

This is $f(g(x))$, where $f(\text{stuff}) = (\text{stuff})^4$ and $g(x) = 2x + 1$.

| Step | Breakdown | Rule Used |
| :--- | :--- | :--- |
| **Identify Outer/Inner Derivatives** | $f'(u) = 4u^3$; $g'(x) = 2$ | Power Rule |
| **Apply Chain Rule** | $h'(x) = f'(g(x)) \cdot g'(x)$ | Chain Rule |
| **Substitute** | $h'(x) = 4(2x + 1)^3 \cdot 2$ | |
| **Final Result** | $h'(x) = **8(2x + 1)^3**$ | |