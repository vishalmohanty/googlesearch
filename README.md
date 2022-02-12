# vmgooglesearch
vmgooglesearch is a Python library for searching Google, easily. vmgooglesearch uses requests and BeautifulSoup4 to scrape Google. This is a fork of https://github.com/Nv7-GitHub/googlesearch.

## Installation
To install, run the following command:
```bash
python3 -m pip install vmgooglesearch
```

## usage
To get results for a search term, simply use the search function in vmgooglesearch. For example, to get results for "Google" in Google, just run the following program:
```python
from vmgooglesearch import search
search("Google")
```

## Additional options
vmgooglesearch supports a few additional options. By default, vmgooglesearch returns 10 results. This can be changed. To get a 100 results on Google for example, run the following program.
```python
from vmgooglesearch import search
search("Google", num_results=100)
```
In addition, you can change the language google searches in. For example, to get results in French run the following program:
```python
from vmgooglesearch import search
search("Google", lang="fr")
```
## vmgooglesearch.search
```python
vmgooglesearch.search(str: term, int: num_results=10, str: lang="en") -> list
```

## Location based search
We use WebSearcher's location to `uule` conversion to search based on locations. Refer https://github.com/vishalmohanty/WebSearcher#obtain-location-names
```python
vmgooglesearch.search(str: term, int: num_results=10, location="Boston,Massachusetts,United States")
```
