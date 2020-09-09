# Cartopy

Spatially-informative linear cartograms using least squares adjustment.

## File formats

### Input

One line per edge, four tokens per line, separated by whitespace.
* Node id
* Node id
* Ideal x difference
* Ideal y difference

Node IDs must be integer, but need not be consecutive.

### Output: default

One line per node, three tokens per line, separated by whitespace.
* Node id as it occurs in the input
* x position
* y position.

### Output: Ipe

Draws the network in an Ipe file. Select using ```--ipe'''.

## Example

Go from the raw input to the raw output.

```
cat example/example.in | python3 linca/linca.py
```

Draw as an Ipe file.

```
cat example/example.in | python3 linca/linca.py --scale=32 --ipe > example.ipe
```