---
layout: post
title:  "35k SNP data for Winter SHW NAM population"
date:   2022-12-12 15:43:05 +0000
categories: jekyll update
---
This page contains links to the full 35k breeders' array genotype data for the NIAB Winter Synthetic Hexaploid Wheat (SHW) Nested Association Mapping (NAM) population. 

The data includes SHW derivatives, SHW parents and a number of Robigus replicates. The genotype QC in the axiom software was completed with QC thresholds of DQC = 0.8 and a QC call rate = 90%. An inbred penalty of 4 and a cr-cut off of 96 were used in the SNP calling. The data is in numeric format and was converted from the original axiom call codes (AA, AB, BB and NoCall) format using the following conversion:

`"NoCall" = NA`
`"AA" = 0`
`"AB" = 1`
`"BB" = 2`

The marker calls for all 35,143 SNPs are included. The last 25 columns of the data contain SNP metrics outputted from the axiom software. 

The following table shows the pedigree and information of genotypes in the data: 

 | First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |





You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
