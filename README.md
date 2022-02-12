# vm_googlesearch
vm_googlesearch is a Python library for searching Google, easily. vm_googlesearch uses requests and BeautifulSoup4 to scrape Google. This is a fork of https://github.com/Nv7-GitHub/googlesearch.

## Installation
To install, run the following command:
```bash
python3 -m pip install vm_googlesearch
```

## usage
To get results for a search term, simply use the search function in vm_googlesearch. For example, to get results for "Google" in Google, just run the following program:
```python
from vm_googlesearch import search
search("Google")
```

## Additional options
vm_googlesearch supports a few additional options. By default, vm_googlesearch returns 10 results. This can be changed. To get a 100 results on Google for example, run the following program.
```python
from vm_googlesearch import search
search("Google", num_results=100)
```
In addition, you can change the language google searches in. For example, to get results in French run the following program:
```python
from vm_googlesearch import search
search("Google", lang="fr")
```
## vm_googlesearch.search
```python
vm_googlesearch.search(str: term, int: num_results=10, str: lang="en") -> list
```

## Location based search
We use WebSearcher's location to `uule` conversion to search based on locations. Refer https://github.com/vishalmohanty/WebSearcher#obtain-location-names
```python
vm_googlesearch.search(str: term, int: num_results=10, location="Boston,Massachusetts,United States")
```
