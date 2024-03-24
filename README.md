# EvoLaMus labs
Lab assignments for the Evolution of Language & Music course.

Website: [clclab.github.io/elm-labs](https://clclab.github.io/elm-labs/intro.html)

## Making edits
To make edits in the lab assignments and publish them to the website, you need to:
1. Clone this repository locally:
   ```
   git clone git@github.com:clclab/elm-labs.git
   cd elm-labs
   ```
2. Install [jupyter-book](https://jupyterbook.org/en/stable/intro.html) and [ghp-import](https://github.com/c-w/ghp-import)
   ```
   pip install -U jupyter-book
   pip install ghp-import
   ```
3. Make sure your local files are up-to-date with the ones in this repository:
   ```
   git pull
   ```
4. \*Make the changes to the local files on your computer\*
5. Rebuild the book:
   ```
   jupyter-book build --all book
   ```
6. Add, commit and push the changes to this repository:
   ```
   git add *
   git commit -m 'some edits'
   git push
   ```
7. Send the updated html to the [gh-pages](https://github.com/clclab/elm-labs/tree/gh-pages) branch (this is what gets published to the website):
   ```
   ghp-import -n -p -f book/_build/html
   ```
8. Typically the changes should be live after a few minutes. If you don't see the changes, try opening the website in an incognito window; if the changes do show up there, it should be fine. If not, check the [Actions tab](https://github.com/clclab/elm-labs/actions) of this repository for build fails.

Steps 1 and 2 only need to be done once; then repeat steps 3 through 7 anytime you want to make new edits.
