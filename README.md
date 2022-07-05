# waldl

Browse [wallhaven](https://wallhaven.cc/) using `sxiv`


## Usage
```
waldl XXX YYY Z <query>
```
> X in `XXX` takes value either 1(on) or 0(off) for `purity` [ sfw/sketchy/nsfw ] NSFW requires a valid API key\
> Y in `YYY` takes value either 1(on) or 0(off) for `categories` [ general/anime/people ]

> `Z` takes positive values (>0) for number of pages

> Leave query empty to use `dmenu`, default values have been set for first,second and third arguments.


- Select wallpapers by marking them using `m` in `sxiv`.
- Quit `sxiv` using `q`.

Selected images would be downloaded. The default download directory is

	~/.local/share/wallhaven

Defaults can be changed by changing the user variables, in the start of the
script.

**Example**
```
waldl 100 010 3 zero two
```

## Dependencies

* sxiv
* jq
* curl
* dmenu ( *optional* )
