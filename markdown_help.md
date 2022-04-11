# Markdown help

## Contents
{: .no_toc}

- TOC
{:toc}

### Markdown within HTML blocks

==Causing problems with `<details` tag===

Markdown is usually ignored within HTML blocks.

<https://stackoverflow.com/questions/38417624/table-of-contents-using-jekyll-and-kramdown>

Use this in _config.yml

```
kramdown:
  parse_block_html: true
```

Also the `parse_block_html` control here: <https://kramdown.gettalong.org/quickref.html>

## Resources

* [HTML tag whitelist](https://gist.github.com/seanh/13a93686bf4c2cb16e658b3cf96807f2)
* [GFM spec](https://github.github.com/gfm/#list-items)

## Audio

<audio controls><source src="amen.mp3"></audio>

## Lists within `<details>`

You must close `<li>` tags within `<details>` tags

<details>
	<ul>
		<li>Please close</li>
		<li>These list items</li>
	</ul>
</details>


## Youtube video controls

<iframe width="560" height="315" src="https://www.youtube.com/embed/qJi03NqXfk8?start=13&end=100" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Continuing numbering

4. Starting numbering like this works in Github, but not pages.


<ol start=4>
<li>Use HTML on pages to customise <code>ol</code> starting number</li>
<li>But remember to close the <code>li</code> tag</li>
</ol>