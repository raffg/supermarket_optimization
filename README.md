# Supermarket Optimization

This script identifies association rules based on existing records of buyer’s transactions at a supermarket. The input is a whitespace delimited data file, where each row records the SKU numbers of items in a single transaction. The script finds the most common items sold together. The set size for the common items is defined in the variable `item_set_size`, and a parameter `sigma` defines the minimum number of occurances of each set to return. Default values are 3 for `item_set_size` and 4 for `sigma`.

## Usage

From the command line, run the script on the default dataset (`retail_25k.dat`) and using the default values for `item_set_size = 3` and `sigma = 4` using the command

`python supermarket_optimization.py`

An alternate dataset and different values for the model parameters can be specified by adding arguments (the order must be `filename, item_set_size, sigma`), such as

`python supermarket_optimization.py retail_25k.dat 3 4`

See the [Python script](supermarket_optmization.py) for commented code and the [Jupyter notebook](supermarket_optimization.ipynb) for expected output.

## Example Output

Running the script on the `retail_25k.dat` dataset with `item_set_size = 3` and `sigma = 4` results in the file [output.csv](output.csv).

