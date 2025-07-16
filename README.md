# Gradient_Descent

<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
  <img src="https://img.shields.io/badge/Matplotlib-EE6633?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter" />
</div>

<h1 align="center" style="color: #4CAF50; font-family: 'Segoe UI', sans-serif; font-size: 3.5em; text-shadow: 2px 2px 4px rgba(0,0,0,0.2);">
  <br>
  <a href="https://github.com/your-username/gradient-descent-visualization">
    <img src="https://placehold.co/600x200/4CAF50/FFFFFF?text=Gradient+Descent+Visualization" alt="Gradient Descent Visualization Banner" style="border-radius: 15px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);">
  </a>
  <br>
  📉 Gradient Descent Visualization 📈
  <br>
</h1>

<p align="center" style="font-size: 1.2em; color: #555; max-width: 800px; margin: 0 auto; line-height: 1.6;">
  Welcome to the **Gradient Descent Visualization** project! This Jupyter Notebook provides a clear and interactive demonstration of the Gradient Descent algorithm in action. Witness how this fundamental optimization technique iteratively finds the minimum of a function, complete with dynamic 3D plots showing the descent path. Ideal for anyone wanting to grasp the core concepts of optimization in machine learning! ✨
</p>

<br>

<details style="background-color: #F0FFF0; border-left: 5px solid #4CAF50; padding: 15px; border-radius: 8px; margin: 20px auto; max-width: 700px; box-shadow: 0 2px 10px rgba(0,0,0,0.1);">
  <summary style="font-size: 1.3em; font-weight: bold; color: #333; cursor: pointer;">Table of Contents</summary>
  <ol style="list-style-type: decimal; padding-left: 25px; line-height: 1.8;">
    <li><a href="#about-the-project" style="color: #4CAF50; text-decoration: none;">📚 About The Project</a></li>
    <li><a href="#how-it-works" style="color: #4CAF50; text-decoration: none;">⚙️ How It Works</a></li>
    <li><a href="#features" style="color: #4CAF50; text-decoration: none;">🎯 Features</a></li>
    <li><a href="#prerequisites" style="color: #4CAF50; text-decoration: none;">🛠️ Prerequisites</a></li>
    <li><a href="#how-to-run" style="color: #4CAF50; text-decoration: none;">📋 How to Run</a></li>
    <li><a href="#example-output" style="color: #4CAF50; text-decoration: none;">📊 Example Output</a></li>
    <li><a href="#code-breakdown" style="color: #4CAF50; text-decoration: none;">🧠 Code Breakdown</a></li>
    <li><a href="#customization-ideas" style="color: #4CAF50; text-decoration: none;">💡 Customization Ideas</a></li>
    <li><a href="#contribute" style="color: #4CAF50; text-decoration: none;">🤝 Contribute</a></li>
  </ol>
</details>

---

<h2 id="about-the-project" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFD700; padding-bottom: 10px;">
  📚 About The Project
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  This project offers a visual and intuitive understanding of the **Gradient Descent algorithm**. It demonstrates how this iterative optimization algorithm works by minimizing a simple 2D quadratic function (<code>f(x, y) = x^2 + y^2</code>). You'll see the algorithm converge step-by-step towards the function's minimum, illustrated through dynamic 3D plots. This notebook is an excellent educational resource for anyone learning about optimization in machine learning and deep learning contexts.
</p>

---

<h2 id="how-it-works" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFD700; padding-bottom: 10px;">
  ⚙️ How It Works
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  The Gradient Descent algorithm works by taking repeated steps in the opposite direction of the gradient (or approximate gradient) of the function at the current point.
</p>
<ol style="list-style-type: decimal; padding-left: 20px; font-size: 1.1em; color: #444; line-height: 1.8;">
  <li style="margin-bottom: 10px;">
    <strong style="color: #4CAF50;">Define the Function:</strong> A simple convex function <code>f(x, y) = x^2 + y^2</code> is chosen for clear visualization.
  </li>
  <li style="margin-bottom: 10px;">
    <strong style="color: #4CAF50;">Calculate Gradients:</strong> The partial derivatives (gradients) of the function with respect to <code>x</code> and <code>y</code> are computed.
  </li>
  <li style="margin-bottom: 10px;">
    <strong style="color: #4CAF50;">Initialize Parameters:</strong> Start from an arbitrary point (<code>x, y</code>) on the function's surface.
  </li>
  <li style="margin-bottom: 10px;">
    <strong style="color: #4CAF50;">Iterative Updates:</strong> In each iteration, the parameters <code>x</code> and <code>y</code> are updated by subtracting a fraction (determined by the <code>learning_rate</code>) of their respective gradients.
    <br><br>
    <code>x_new = x_old - learning_rate * (∂f/∂x)</code><br>
    <code>y_new = y_old - learning_rate * (∂f/∂y)</code>
  </li>
  <li style="margin-bottom: 10px;">
    <strong style="color: #4CAF50;">Convergence:</strong> The process continues for a set number of iterations, gradually moving towards the function's minimum.
  </li>
</ol>

---

<h2 id="features" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFD700; padding-bottom: 10px;">
  🎯 Features
</h2>
<ul style="list-style-type: none; padding: 0; font-size: 1.1em; color: #444;">
  <li style="margin-bottom: 15px; background-color: #E8F5E9; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #4CAF50;">📉 Customizable Parameters:</strong> Easily adjust the initial starting point, learning rate, and number of iterations to observe their impact on convergence.
  </li>
  <li style="margin-bottom: 15px; background-color: #E8F5E9; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #4CAF50;">✨ 3D Surface Plot:</strong> Visualize the objective function as a vibrant 3D surface, providing a clear landscape for optimization.
  </li>
  <li style="margin-bottom: 15px; background-color: #E8F5E9; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #4CAF50;">🚶‍♂️ Descent Path Visualization:</strong> Observe the iterative path taken by the gradient descent algorithm directly on the 3D surface plot.
  </li>
  <li style="margin-bottom: 15px; background-color: #E8F5E9; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #4CAF50;">📈 Convergence Tracking:</strong> The notebook tracks the function value at each step, showcasing the optimization process.
  </li>
  <li style="margin-bottom: 15px; background-color: #E8F5E9; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #4CAF50;">✍️ Well-Commented Code:</strong> Understand each line of code with clear explanations, making it an ideal learning tool.
  </li>
</ul>

---

<h2 id="prerequisites" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFD700; padding-bottom: 10px;">
  🛠️ Prerequisites
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  To run this project, ensure you have the following installed:
</p>
<ul style="list-style-type: disc; padding-left: 20px; font-size: 1.1em; color: #444;">
  <li><strong style="color: #4CAF50;">Python 3.x</strong></li>
  <li><strong style="color: #4CAF50;">Jupyter Notebook</strong></li>
  <li>Required Libraries:
    <pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code>pip install numpy matplotlib</code></pre>
  </li>
  <li><strong style="color: #4CAF50;">Google Colab</strong> (optional, for running the notebook in the cloud)</li>
</ul>

---

<h2 id="how-to-run" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFD700; padding-bottom: 10px;">
  📋 How to Run
</h2>
<ol style="list-style-type: decimal; padding-left: 20px; font-size: 1.1em; color: #444; line-height: 1.8;">
  <li style="margin-bottom: 10px;">
    <strong style="color: #4CAF50;">Clone or Download the Notebook:</strong>
    <p style="margin-top: 5px;">Download <code>Gradient_descent.ipynb</code> from this repository.</p>
    <p style="margin-top: 5px;">Alternatively, open it directly in <a href="https://colab.research.google.com/" style="color: #4CAF50; text-decoration: none;">Google Colab</a>.</p>
  </li>
  <li style="margin-bottom: 10px;">
    <strong style="color: #4CAF50;">Install Dependencies:</strong>
    <pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code>pip install numpy matplotlib</code></pre>
  </li>
  <li style="margin-bottom: 10px;">
    <strong style="color: #4CAF50;">Run the Notebook:</strong>
    <p style="margin-top: 5px;">Open <code>Gradient_descent.ipynb</code> in Jupyter or Colab.</p>
    <p style="margin-top: 5px;">Execute each cell sequentially to visualize the gradient descent process! ✨</p>
  </li>
  <li style="margin-bottom: 10px;">
    <strong style="color: #4CAF50;">Experiment:</strong>
    <p style="margin-top: 5px;">Modify the <code>start_x</code>, <code>start_y</code>, <code>learning_rate</code>, and <code>num_iterations</code> variables to see how they affect the descent path and convergence.</p>
  </li>
</ol>

---

<h2 id="example-output" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFD700; padding-bottom: 10px;">
  📊 Example Output
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  When you run the notebook, you'll see a 3D plot of the function <code>f(x, y) = x^2 + y^2</code> with the path of the gradient descent algorithm overlaid, visually demonstrating its convergence to the minimum.
</p>
<div style="text-align: center; background-color: #F8F8F8; padding: 15px; border-radius: 10px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin-top: 20px;">
  <h3 style="color: #4CAF50; font-size: 1.5em; margin-bottom: 10px;">Gradient Descent Path on 3D Surface:</h3>
  <img src="https://placehold.co/500x350/C8E6C9/333333?text=Gradient+Descent+Plot" alt="Gradient Descent Plot Placeholder" style="width: 100%; max-width: 500px; height: auto; border-radius: 8px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #666; margin-top: 10px;">
    This visualization illustrates how the algorithm navigates the function's surface to find the optimal point.
  </p>
</div>

---

<h2 id="code-breakdown" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFD700; padding-bottom: 10px;">
  🧠 Code Breakdown
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  Here’s a quick overview of the key functions and their roles:
</p>

<h3 style="color: #4CAF50; font-size: 1.8em; margin-top: 25px;">Objective Function `f(x, y)`:</h3>
<pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code><span style="color: #569CD6;">def</span> <span style="color: #6A9955;">f</span>(<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>):
    <span style="color: #C586C0;">return</span> <span style="color: #9CDCFE;">x</span>**<span style="color: #B5CEA8;">2</span> <span style="color: #C586C0;">+</span> <span style="color: #9CDCFE;">y</span>**<span style="color: #B5CEA8;">2</span></code></pre>

<h3 style="color: #4CAF50; font-size: 1.8em; margin-top: 25px;">Gradient Functions `df_dx(x, y)` and `df_dy(x, y)`:</h3>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  Compute the partial derivatives of the function, which represent the slope in each dimension.
</p>
<pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code><span style="color: #569CD6;">def</span> <span style="color: #6A9955;">df_dx</span>(<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>):
    <span style="color: #C586C0;">return</span> <span style="color: #B5CEA8;">2</span> <span style="color: #C586C0;">*</span> <span style="color: #9CDCFE;">x</span>

<span style="color: #569CD6;">def</span> <span style="color: #6A9955;">df_dy</span>(<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>):
    <span style="color: #C586C0;">return</span> <span style="color: #B5CEA8;">2</span> <span style="color: #C586C0;">*</span> <span style="color: #9CDCFE;">y</span></code></pre>

<h3 style="color: #4CAF50; font-size: 1.8em; margin-top: 25px;">Gradient Descent Core `gradient_descent(...)`:</h3>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  The main function that performs the iterative optimization.
</p>
<pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code><span style="color: #569CD6;">def</span> <span style="color: #6A9955;">gradient_descent</span>(<span style="color: #9CDCFE;">start_x</span>, <span style="color: #9CDCFE;">start_y</span>, <span style="color: #9CDCFE;">learning_rate</span>, <span style="color: #9CDCFE;">num_iterations</span>):
    <span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">start_x</span>, <span style="color: #9CDCFE;">start_y</span>
    <span style="color: #9CDCFE;">history</span> <span style="color: #CE9178;">=</span> [(<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>, <span style="color: #9CDCFE;">f</span>(<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>))]

    <span style="color: #569CD6;">for</span> <span style="color: #9CDCFE;">_</span> <span style="color: #CE9178;">in</span> <span style="color: #569CD6;">range</span>(<span style="color: #9CDCFE;">num_iterations</span>):
        <span style="color: #9CDCFE;">grad_x</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">df_dx</span>(<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>)
        <span style="color: #9CDCFE;">grad_y</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">df_dy</span>(<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>)

        <span style="color: #9CDCFE;">x</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">x</span> <span style="color: #CE9178;">-</span> <span style="color: #9CDCFE;">learning_rate</span> <span style="color: #CE9178;">*</span> <span style="color: #9CDCFE;">grad_x</span>
        <span style="color: #9CDCFE;">y</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">y</span> <span style="color: #CE9178;">-</span> <span style="color: #9CDCFE;">learning_rate</span> <span style="color: #CE9178;">*</span> <span style="color: #9CDCFE;">grad_y</span>

        <span style="color: #9CDCFE;">history.append</span>((<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>, <span style="color: #9CDCFE;">f</span>(<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>)))

    <span style="color: #C586C0;">return</span> <span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>, <span style="color: #9CDCFE;">f</span>(<span style="color: #9CDCFE;">x</span>, <span style="color: #9CDCFE;">y</span>), <span style="color: #9CDCFE;">history</span></code></pre>

---

<h2 id="customization-ideas" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFD700; padding-bottom: 10px;">
  💡 Customization Ideas
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  Want to delve deeper into optimization? Here are some ways to extend this project:
</p>
<ul style="list-style-type: none; padding: 0; font-size: 1.1em; color: #444;">
  <li style="margin-bottom: 15px; background-color: #E8F5E9; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #4CAF50;">📈 Different Functions:</strong> Implement gradient descent for more complex functions (e.g., non-convex, higher dimensions).
  </li>
  <li style="margin-bottom: 15px; background-color: #E8F5E9; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #4CAF50;">🔄 Advanced Optimizers:</strong> Add implementations of other optimization algorithms like Momentum, Adagrad, RMSprop, or Adam for comparison.
  </li>
  <li style="margin-bottom: 15px; background-color: #E8F5E9; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #4CAF50;">🎨 Interactive Plotting:</strong> Use interactive plotting libraries (e.g., Plotly) to allow real-time parameter changes and visualize convergence dynamically.
  </li>
  <li style="margin-bottom: 15px; background-color: #E8F5E9; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #4CAF50;">📊 Performance Metrics:</strong> Track and plot the function value over iterations to visualize the convergence curve.
  </li>
</ul>

---

<h2 id="contribute" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFD700; padding-bottom: 10px;">
  🤝 Contribute
</h2>
<p align="center" style="font-size: 1.2em; color: #555; max-width: 800px; margin: 0 auto; line-height: 1.6;">
  Contributions are highly valued! If you have ideas for improvements, new features, or different optimization algorithms to visualize, please feel free to open an issue or submit a pull request. Let’s explore the world of optimization together! 🚀
</p>
<p align="center" style="font-size: 1.2em; color: #555; max-width: 800px; margin: 15px auto 0; line-height: 1.6;">
  Star this repo if you find it helpful! ⭐
</p>
<p align="center" style="font-size: 1em; color: #777; margin-top: 30px;">
  Created with 💖 by Chirag
</p>
