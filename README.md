<h1 align = "center">Wordle Solver</h1>

This is a portable version of 3B1B's visualized solver for [wordle](https://www.powerlanguage.co.uk/wordle/) with all bugs fixed.

## Prerequisites

For more details like `FFmpeg` or LaTeX distribution, see [manim installation](https://github.com/3b1b/manim#installation) .

```shell
# Install manimgl
pip install manimgl

# Try it out
manimgl
```

## Usage

1. (must) Create an empty folder `data/wordle` .

2. Run `wordle.py` to get `data/wordle/pattern_matrix.npy` :

   ```shell
   python wordle.py
   ```

   This step may take some minutes, but the results will be saved so that it is only needed for the first time.

3. Run wordle-solver:

   ```shell
   manimgl wordle.py InitialDemo
   ```

   Then input the suggested start word `crane` on the pop-up window with its feedback `gray` / `yellow` / `green` mapped to `0` / `1` / `2` , finished with `Enter` , loop until the problem is cracked.

![example](https://github.com/Tequila-Sunrise/Image-Hosting/blob/main/Wordle-Solver/wordle-solver.jpg)
