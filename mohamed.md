# Calculus Final Project: Area Approximation with Riemann Sums

## Learning Intention
Investigate how Riemann Sums and Integrals approximate the area under a curve. Analyze how accuracy changes with more subdivisions (n).

## Example 1: Function Details

### 1. Function: 
\[ f(x) = x^2 \]
### 2. Interval: 
\[ [1, 4] \]
### 3. Number of Subdivisions (n):
\[ n = 4 \]

### Left Riemann Sum
- Subinterval width: \( \Delta x = \frac{4-1}{4} = 0.75 \)
- Left endpoints: \( x_0 = 1, x_1 = 1.75, x_2 = 2.5, x_3 = 3.25 \)
- Function values: \( f(1) = 1, f(1.75) = 3.0625, f(2.5) = 6.25, f(3.25) = 10.5625 \)
- Approximation:
\[ L_4 = 0.75 (1 + 3.0625 + 6.25 + 10.5625) = 15.7031 \]

### Right Riemann Sum
- Right endpoints: \( x_1 = 1.75, x_2 = 2.5, x_3 = 3.25, x_4 = 4 \)
- Function values: \( f(1.75) = 3.0625, f(2.5) = 6.25, f(3.25) = 10.5625, f(4) = 16 \)
- Approximation:
\[ R_4 = 0.75 (3.0625 + 6.25 + 10.5625 + 16) = 27.7031 \]

### Exact Area Calculation
Definite integral:
\[ \int_{1}^{4} x^2 dx \]
Solving:
\[ \frac{x^3}{3} \Bigg|_1^4 = \frac{64}{3} - \frac{1}{3} = \frac{63}{3} = 21 \]

### Comparison and Analysis
- **Left Riemann Sum:** \( L_4 = 15.7031 \)
- **Right Riemann Sum:** \( R_4 = 27.7031 \)
- **Exact Area:** \( 21 \)

As n increases, the approximations improve since the rectangles better conform to the curve's shape.

---

## Example 2: Function Details

### 1. Function: 
\[ f(x) = \sin(x) \]
### 2. Interval: 
\[ [0, \pi] \]
### 3. Number of Subdivisions (n):
\[ n = 6 \]

### Left Riemann Sum
- Subinterval width: \( \Delta x = \frac{\pi - 0}{6} = \frac{\pi}{6} \)
- Compute function values at left endpoints and find sum

### Right Riemann Sum
- Compute function values at right endpoints and find sum

### Exact Area Calculation
Definite integral:
\[ \int_{0}^{\pi} \sin(x) dx \]
Solving:
\[ -\cos(x) \Bigg|_0^{\pi} = -(-1) - (-1) = 2 \]

### Comparison and Analysis
- **Left Riemann Sum:** Approximate value
- **Right Riemann Sum:** Approximate value
- **Exact Area:** \( 2 \)

Increasing subdivisions improves accuracy.

---

