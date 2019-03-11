# Hexo-WordCount-Arabic

## Installation

```bash
yarn add hexo-wordcount
# or
npm i --save hexo-wordcount
```

## Usage

###  WordCount


```js
wordcount(post.content)
```

###  Min2Read

```js
min2read(post.content)
```

 Set Reading Speed:

```js
min2read(post.content, {cn: 300,ar:200, en: 160})
// p.s. (v3.0.0 added)
```

###  TotalCount

```js
totalcount(site)
```

## Demo

### Swig

Post Count:

```swig
   <span class="post-count">{{ wordcount(post.content) }}</span>
```

Post Minutes to Read:

```swig
   <span class="post-count">{{ min2read(post.content) }}</span>
```

Total Count:

```swig
   <span class="post-count">{{ totalcount(site) }}</span>
```

### Ejs

Post Count:

```ejs
   <span class="post-count"><%= wordcount(post.content) %></span>
```

Post Minutes to Read:

```ejs
   <span class="post-count"><%= min2read(post.content) %></span>
```

Total Count:

```ejs
   <span class="post-count"><%= totalcount(site) %></span>
```

### Jade

Post Count:

```jade
   span.post-count= wordcount(post.content)
```

Post Minutes to Read:

```jade
    span.post-count= min2read(post.content)
```


Total Count:

```swig
   span.post-count= totalcount(site)
```


## LICENSE

MIT
