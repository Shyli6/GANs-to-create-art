# Monet-Style Image Generation using CycleGAN

This project demonstrates how to use a pre-trained CycleGAN model to transform real-world landscape images into Monet-style paintings. It was developed as part of a Deep Learning mini-project.

---

## Project Structure

```
GANS_mini_project_image.ipynb     # Main notebook
leaderboard score_kaggle          # Kaggle score card
```

---

## Model Details

- **Architecture:** CycleGAN
- **Generator Used:** Monet → Photo (`gen_F_epoch_10.h5`)
- **Input:** Real-world photo images
- **Output:** Monet-style image translations

---

## How to Run

1. **Clone this repo:**

   ```bash
   git clone https://github.com/your-username/monet-style-cyclegan.git
   cd monet-style-cyclegan
   ```

2. **Install dependencies:**

   This project uses TensorFlow 2.x, NumPy, and Matplotlib.

   ```bash
   pip install tensorflow numpy matplotlib
   ```

3. **Download Sample Test Images:**

   - Visit the Kaggle competition:  
     [I'm Something of a Painter Myself](https://www.kaggle.com/competitions/gan-getting-started/data)
   - Download the `test_photo_v2.zip` file (or equivalent)
   - Extract and place images into a folder named `images/`

4. **Update Image Path in Notebook:**

   In the notebook, locate the line:

   ```python
   input_image_dir = "/path/to/your/images"
   ```

   Replace it with your actual path, for example:

   ```python
   input_image_dir = "./images"
   ```

5. **Run the Notebook:**

   Use Jupyter or VSCode to run `GANS_mini_project_image.ipynb`.  
   This will display several generated Monet-style images inline using `matplotlib`.

---

## Acknowledgments

- Pretrained models from the Kaggle dataset
- Based on CycleGAN paper: [Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks](https://arxiv.org/abs/1703.10593)

---

## Notes

- The notebook avoids reprocessing images if they are already generated.
- Ensure image file types are `.jpg` and correctly formatted before inference.
- You may need to use Git LFS if uploading large models (`*.h5`) to GitHub.

---

## GITHUB URL

https://github.com/Shyli6/GANs-to-create-art.git