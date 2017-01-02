<!--tags: help, start -->

# Searching
Did you type full file path (`search.md`) to open this document? Did you selected it by mouse?
There are other much more simple options to find documents. You can find this document by typing `se` | `help` | `search start` | `action`.
Why? Let's figure it out.

> Use keyboard to be as productive as possible. Here is a list of shortcusts:
> * `enter` (when input field is selected) - try to open document by path or make fulltext request
> * `arrow down` / `arrow up` - select next / prev document from suggestions
> * `ctrl`+`1` - select input field

## Into
You can find document in two ways:
* by filter - filter documents by path and tags - works on client - very fast
* or by fulltext search - filter documents by fulltext search over content - works on server - a little bit slower.

## Searching
Searching is simple - just type text from path / tags / content, hit `enter` and get list of approriate documents.

Searching allows you to find this document by typing `how to search` | `shortcusts`

## Filtering
Filtering is very fast but works only on document path and tags.
It has some specific rules, which allow you filter documents much faster:

* We split your request into words (by upper case, `-`, `.`). E.g. `helloWorld.md` will be splited into `hello`, `world` and `md`
* We do the same thing with document title / tags
* After that we try to find documents which has all words from your request in title / tags. To compare words we use `startsWith` rule

This technic allows you to type only parts of the words and get response.
E.g. you can find document `helloWorld.md` by typing `he wo` (`hello` starts from `he`, `world` starts from `wo`)

Filtering allows you to find this document by typing `search` | `search help` | `help start`

## Summary
Here is a summary of different ways to find document. Use them and you will find your documents very fast!

| Type | How to |
| --- | --- |
| open by full path name  | type `search.md` > `enter`  |
| filter by path | type `search` (or `se` \| `se.md` \| `seMd`) > `arrow down` (to select from results) > `enter` |
| filter by tags | type `help` (or `start` \| `he sta`) > `arrow down` > `enter` |
| filter by combination | type `start search` (or `search help` \| `se he`) > `arrow down` > `enter` |
| fulltext search by content | type `action` > `enter` > `arrow down` > `enter` |