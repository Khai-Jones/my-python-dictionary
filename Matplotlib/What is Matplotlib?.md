# What is Matplotlib 

Matplotlib is a python library used to create visual, static or interactive visualizations. It is highly customizable (maybe too customizable) and is built on NumPy, making it efficient for numerical and scientific data visualization. 

It is imported as: 

```python
import matplotlib.pyplot as plt
```

Every plot can be based upon this template:

``` python
import matplotlib.pyplot as plt

# 1. Create figure and axes
fig, ax = plt.subplots(figsize=(8, 5))  # Width x Height in inches

# 2. Plot data
x = [...]  # Your x-axis values
y = [...]  # Your y-axis values
ax.plot(x, y, label='Sample Data', color='blue', marker='o')  # Change to ax.bar, ax.scatter, etc. as needed

# 3. Add plot essentials
ax.set_title('Plot Title')         # Always add a descriptive title
ax.set_xlabel('X-axis Label')      # Label your x-axis
ax.set_ylabel('Y-axis Label')      # Label your y-axis
ax.legend()                        # Add if there's a label
ax.grid(True)                      # Optional but helpful for readability

# 4. Adjust layout and display
plt.tight_layout()                 # Avoid label/element overlap
plt.show()

```
To save a plot as an image you can use the plt.savefig function: 
``` python
plt.savefig('my_plot.png', dpi=300, bbox_inches='tight')  # Save before plt.show()
```
#### Common plot types in Matplotlib

Absolutely! Here's your full **Matplotlib notes module**, now expanded to include all major **plot types**, their **purpose**, and **how to implement each one** using the same base template structure. This version is ideal for studying, teaching, or practical reference.

---
## 📊 Plot Types in Matplotlib

| Plot Type          | Method                           | Description                                               |
| ------------------ | -------------------------------- | --------------------------------------------------------- |
| **Line Plot**      | `ax.plot(x, y)`                  | Shows trends or change over continuous intervals.         |
| **Bar Plot**       | `ax.bar(x, y)`                   | Vertical bars to compare categories.                      |
| **Horizontal Bar** | `ax.barh(x, y)`                  | Same as bar plot, but horizontal layout.                  |
| **Scatter Plot**   | `ax.scatter(x, y)`               | Points showing distribution or correlation.               |
| **Histogram**      | `ax.hist(data, bins=20)`         | Frequency distribution of continuous data.                |
| **Box Plot**       | `ax.boxplot(data)`               | Displays median, quartiles, outliers.                     |
| **Pie Chart**      | `plt.pie(sizes)`                 | Part-to-whole relationships. Only with `plt`, not `ax`.   |
| **Stacked Area**   | `ax.stackplot(x, y1, y2, ...)`   | Area under multiple lines stacked cumulatively.           |
| **Step Plot**      | `ax.step(x, y)`                  | Line with discrete jumps, used in control or state data.  |
| **Fill Between**   | `ax.fill_between(x, y1, y2)`     | Fills space between two curves or a line and x-axis.      |
| **Error Bar Plot** | `ax.errorbar(x, y, yerr=errors)` | Adds vertical or horizontal error bars.                   |
| **Hexbin Plot**    | `ax.hexbin(x, y)`                | Like a 2D histogram using hexagonal bins.                 |
| **2D Histogram**   | `ax.hist2d(x, y)`                | Shows density using square color bins.                    |
| **Image Plot**     | `ax.imshow(image)`               | Displays 2D arrays as an image (e.g. grayscale, heatmap). |
| **Contour Plot**   | `ax.contour(X, Y, Z)`            | Lines connecting equal values in 3D surface (like a map). |
| **Filled Contour** | `ax.contourf(X, Y, Z)`           | Same as contour but areas are filled with color.          |
| **Quiver Plot**    | `ax.quiver(X, Y, U, V)`          | Shows vector fields (direction and magnitude).            |
| **Stream Plot**    | `ax.streamplot(X, Y, U, V)`      | Flow lines for vector fields (e.g. wind or fluid motion). |

---