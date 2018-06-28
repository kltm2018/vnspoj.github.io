# Tutorial SPOJ

Hướng dẫn và chia sẻ lời giải cho các problems trên vn.spoj.com.

## Development

+ Make sure you have Ruby install in your computer, if not
```bash
sudo apt install ruby ruby-dev
```
+ Install jekyll theme [here](https://jekyllrb.com/) or simply type
```bash
gem install bundler jekyll
```
+ Install packages in gem. You'll be required password to install packages. If you get error requiring "Make sure that `gem install ...`", please execute the command with `sudo`.
```bash
bundle install
```
+ Serve jekyll server on localhost, and open `localhost:4000/` to view the site.
```bash
bundle exec jekyll serve
```

## Contribution

### Solution files
The solution files (source code) should be in the repository [https://github.com/vnspoj/solution](https://github.com/vnspoj/solution). You will add your files which name is formatted as `[problem_code].cpp` or `[problem_code].java` in directory `src/*`. 


Example, if the problem you solved is `NKCITY` (the problem url will be [https://vn.spoj.com/problems/NKCITY/](https://vn.spoj.com/problems/NKCITY/)), then your solution file is `NKCITY.cpp` or `NKCITY.java`, and it'll be added to `src`, the path is `src/NKCITY.cpp` (or `.java`). And the file will be served staticly at [https://vnspoj.github.io/solution/src/NKCITY.cpp](https://vnspoj.github.io/solution/src/NKCITY.cpp)


### Tutorial
The tutorial should be in this repository [https://github.com/vnspoj/vnspoj.github.io](https://github.com/vnspoj/vnspoj.github.io). Open directory `_posts` and add new file `markdown` with extension `.md` or `.markdown`, which name is formatted as `yyyy-mm-dd-[problem_code].md` (or `.markdown`), with `yyyy-mm-dd` is year, month, date you write the tutorial and `[problem_code]` as above.


In the new file, the structure should be:

```md
---
layout: post
title:  "NKCITY - Xây dựng thành phố"
categories: [mst, kruskal]
code: NKCITY
src: NKCITY.cpp
---

[Your content here]

```

In the above file, you should change the `title`, `categories`, `code` and `src`, with `src` is name of file you publish in the repository `solution`.


If you need static files (such as iamge, pdf, or bla bla), you can add in the directory `static`, and the url becomes `https://vnspoj.github.io/static/[path/to/your/file]`

### Add new category
+ Add new file in `category` as the others in the directory.
+ In directory `_posts/tips`, add new file as the others.

### Use with Math type
If in post you need use math type, you should have `use_math: true` in top file, such as:
```bash
---
layout: post
title:  "SPSEQ - Sequences"
categories: [dp, lis]
code: SPSEQ
src: SPSEQ.cpp
use_math: true
---
```

For inline math type: 
```
That is inline:  \\( 1/x^{n} \\)
```

For block math type: 
```
That is block \\[ \frac{1}{n^{2}} \\]
```
