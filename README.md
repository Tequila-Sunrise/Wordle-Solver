<h1 align = "center">Wordle Solver</h1>

This is a portable version of [3B1B's visualized solver](https://github.com/3b1b/videos/tree/master/_2022/wordle) for [wordle](https://www.nytimes.com/games/wordle/index.html) with all bugs fixed.

## Prerequisite

For more details like `FFmpeg` or LaTeX distribution, see [manim installation](https://github.com/3b1b/manim#installation) .

```shell
# Install manimgl
pip install manimgl

# Try it out
manimgl
```

## Usage

Open terminal under `Wordle-Solver/` :

```shell
manimgl wordle/scenes.py InitialDemo
```

This step may take some minutes for the first time, but the `pattern_matrix.npy` results will be saved under `data/` so that there is no need for generation henceforth.

Then input the suggested start word `SALET` on the pop-up window with its feedback `gray` / `yellow` / `green` mapped to `0` / `1` / `2` , finished with `Enter` , loop until the puzzle is cracked.

Enjoy Wordle Cracker!

## Example

Type in `CRANE` - `01000` - `Enter` , take the top pick word `TORUS` - `01110` - `Enter` ... 

WARNING: The best opening word is no longer `CRANE` but `SALET` , see more details in [reference](#reference) .

![example](https://github.com/Tequila-Sunrise/Image-Hosting/blob/main/Wordle-Solver/wordle-solver.jpg)

## Reference

1. [Solving Wordle using information theory](https://youtu.be/v68zYyaEmEA) by 3B1B.
1. [Oh, wait, actually the best Wordle opener is not “crane”…](https://youtu.be/fRed0Xmc2Wg) by 3B1B.
