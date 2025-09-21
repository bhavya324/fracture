# 🧩 Fractal Annotated Fracture Images

This project generates fracture-like images (or processes real ones), extracts their skeletons, and computes the **fractal dimension** using the **box-counting method**.  
It then produces **annotated images** with bounding boxes and overlays the computed fractal dimension.

---

## 📌 Features
- Generate **synthetic fracture images** (for testing).
- Load and preprocess real images.
- Apply **thresholding & skeletonization**.
- Compute **fractal dimension** (box-counting algorithm).
- Annotate results with bounding boxes + text overlay.
- Visualize results step by step in **Jupyter Notebook**.

---

## 🛠️ Installation

Clone the repository and install the dependencies:

```bash
git clone https://github.com/your-username/fractal-fracture-images.git
cd fractal-fracture-images
pip install -r requirements.txt
```

If you don’t have a requirements.txt, install the dependencies manually:
```bash
pip install numpy scikit-image pillow matplotlib scipy
```

## 🚀 Usage

Run the notebook in Jupyter:

```bash
jupyter notebook fractal_fracture.ipynb
```

Inside the notebook:

1. **Load your own fracture image** or let the script generate a **synthetic fracture image**.
2. The pipeline will automatically:
   - Threshold and skeletonize the fracture  
   - Compute the **fractal dimension** (box-counting method)  
   - Save an **annotated PNG** with bounding box + fractal dimension text
3. Results are displayed side by side for easy comparison:

- **Original / Input**  
- **Binary Thresholded**  
- **Skeleton**  
- **Annotated Output**


## 📐 Fractal Dimension

The **box-counting method** is used to estimate the fractal dimension:

\[
D = - \frac{\Delta \log(N(\varepsilon))}{\Delta \log(\varepsilon)}
\]

Where:

- \( \varepsilon \) = box size  
- \( N(\varepsilon) \) = number of boxes covering fracture pixels


## 📂 Project Structure

```bash
.
├── fractal_fracture.ipynb   # Main notebook
├── README.md                # Project documentation
├── assets/                  # Example output images
└── requirements.txt         # Python dependencies
```
## 🤝 Contributing

Pull requests are welcome!
If you’d like to add new fractal estimation methods or batch-processing support, fork and improve 🚀


