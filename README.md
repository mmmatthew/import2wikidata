# import2wikidata
Script to import Open Data Zurich fountains into wikidata without overwriting existing data. The script generates Quickstatement commands to be run in the online interface `https://tools.wmflabs.org/wikidata-todo/quick_statements.php`.

The project is open source under the GNU Affero General Public License, with a profit contribution agreement applying under restricted conditions. See [COPYING](/COPYING) for information.

## Requirements
- Python 3.3 or higher (https://www.python.org/downloads/release/python-365/)
- Jupyter (http://jupyter.org/install)
- all packages mentioned in the import lines of the Jupyter notebook `zurich_fountains_preprocess.ipynb` (use `pip install [package name]` to install)

## How to run
- Clone this repository to your local machine `git clone https://github.com/mmmatthew/import2wikidata.git`
- Start jupyter from a command window in the directory just created `jupyter notebook'
- In your browser, open `http://localhost:8888/notebooks/zurich_fountains_preprocess.ipynb` (the port may be different)
- Run the script. It should create a file `quickstatement_commands.txt`

## How to use the generated commands
- Go to `https://tools.wmflabs.org/wikidata-todo/quick_statements.php`.
- Authenticate yourself with your Wikidata account.
- Copy and paste the contents of `quickstatement_commands.txt` into the blank field, and run the commands

## Contributions welcome
The WVZ (https://www.wikidata.org/wiki/Q53629101) does not have all that many changes in its base data. Nonetheless does it make sense to cross-check their master-data-set with what is in WikiData.
