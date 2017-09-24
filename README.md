# Citizen.io Organization Protocol

## Wtf is this?
This repository is intended to contain the RFC of the Citizen.io Organization Protocol.

## Current status
The is a draft. It might not be really compliant with RFC standards yet.

## RFC generator
### Why?
The official RFC layout is a bit difficult to write and maintain, as it requires ascii padding everywhere. Because of this, using an RFC generator looks like a good idea. This one should take a simple input format for the content, and then translate it to the official RFC format.

### Using Markdown
Markdown has been choosed because it is a simple and lightweight markup language with plain text formatting syntax. Also, it can be easily converted to the RFC format.

### Markdown to RFC
To convert Markdown format to RFC, here is two simple commands:
* [`kramdown-rfc2629`](https://github.com/cabo/kramdown-rfc2629)
* [`xml2rfc`](https://xml2rfc.tools.ietf.org/)

`kramdown-rfc2629` converts Markdown to XML. `xml2rfc` converts XML to RFC.

### How to convert Markdown to RFC?
#### Installation
```sh
$ sudo gem install kramdown-rfc2629
$ sudo pip install xml2rfc
```

*More informations on the installation inside the previously given links for each command.*

#### Usage
```sh
$ kramdown-rfc2629 rfc-citizen-org-proto.md > rfc-citizen-org-proto.xml && xml2rfc rfc-citizen-org-proto.xml
```
