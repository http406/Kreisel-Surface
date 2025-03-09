# Kreisel-Surface

### **What is the Kreisel Surface in this Code?**  
The **Kreisel Surface** in this code is a parametric surface generated using a mathematical equation. It is visualized as a set of points in 3D space, connected to form a unique shape. The structure is created using a **point cloud** representation in Three.js, where each point is assigned a color based on its position.

The surface rotates around the **Y-axis**, and a background of twinkling stars is added for a space-like effect.

---

### **Understanding the Equation Used in the Code**  
The equation used in the code defines the shape of the Kreisel surface in 3D space using **two parameters**:  
- \( u \) (ranges from -𝜋 to 𝜋 
- \( v \) (ranges from -𝜋 to 𝜋

#### **Equation Breakdown**
The code defines the **parametric equations** for the surface as:

\[
r = r_{\max} \cdot \cos(a \cdot u)
\]

\[
x = r \cdot \sin(a \cdot u) \cdot \cos(3v)
\]

\[
y = r \cdot \sin(a \cdot u) \cdot \sin(3v)
\]

\[
z = r \cdot \cos(a \cdot u)
\]

#### **Explanation of Parameters:**
- \( rmax = 2.0 \) → Maximum radius, which controls the overall size of the shape.
- \( a = 1.0 \) → Scaling factor for parameter \( u \), controlling the oscillation of the radius.
- \( u, v \) → Parametric variables that determine the shape in the **circular and radial** directions.

---

### **What Does This Equation Do?**
1. **Radius Variation**:  
   - \( r = rmax • cos(a • u) \) defines how the distance from the center changes with \( u \).
   - The **cosine function** causes the surface to expand and contract periodically.

2. **3D Positioning**:
   - \( x \) and \( y \) use **sine and cosine** functions of \( v \) to create a rotational effect.
   - The factor **\( 3v \)** creates a **tripled twisting pattern**, giving the surface a spiraling, wavy structure.
   - \( z = r • \cos(a • u) \) ensures the height follows the radius function.

---

### **Visualization of the Kreisel Surface**
- The equation defines a **wave-like spiral shape** with **threefold symmetry** around the **Z-axis**.
- The colors are determined by mapping the **hue (HSL color model)** to the **U parameter**, creating a gradient effect.
- The animation rotates the surface around the **Y-axis** to enhance visualization.
