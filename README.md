# Analytics Challenge

### Data overview
This dataset is a transformed version of the [USDA Food Composition Database](https://ndb.nal.usda.gov/ndb/). It is the major source of food composition data in the United States and provides the foundation for most food composition databases in the public and private sectors. The database provides detailed composition data for components like calories, proteins, vitamins, etc. The database contains three tables: `composition`, `units`, and `conversion`.

The `composition` table is formatted as a series of nutritional measurements:
- `item_id`: unique identifier for each item
- `desc`: The name of the item being measured
- `component`: The nutritional component being measured
- `value`: The value of the measurement

**The measurements are in different units**, depending on the component being measured. The `units` table maps each component to its unit of measurement. The `conversion` table maps each unit of measurement to a decimal conversion factor that converts values of each given unit of measurement to grams.

### Setting up your development environment
Anaconda is a Python distribution that contains a collection of pre-installed, helpful libraries for data analysis. If you don't already have Python installed on your machine, you can follow the instructions [here](https://conda.io/docs/user-guide/install/index.html). If you do already have Python or Anaconda installed, make sure you have the following packages installed and up-to-date: `jupyter`, `pandas`, `sqlite3`.

Finally, clone this repo onto your computer.

### Getting started with this challenge
Once you've cloned the repo, run the Python script `dbgen.py`, which will create and populate the SQLite database, `usda.db` to be used for this analysis. **If you accidentally delete or modify the tables in this database, you can re-run this script to create fresh data.**

Launch a Jupyter Notebook server in the repo folder, and open the file called `notebook.ipynb` in Jupyter. This file will be used for logging your analysis and saving your results.

When you're finished, send us the files `notebook.ipynb` and `solutions.json` (it will be generated by running the final cell in the notebook). Good luck!
