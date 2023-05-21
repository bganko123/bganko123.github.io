# My first blog post - A blog post about blog posts
This is the first of many blog posts, these are new exciting times.
1. TOC
{:toc}
## Setting up the blog
### Making the repository
I set up the blog using the guide posted by fastai -> here is the link [links](https://www.fast.ai/posts/2020-01-16-fast_template.html)
To get started and set up the template, I used this link -> [links](https://github.com/fastai/fast_template/generate)
This generates a repository that will store the blog and your posts. You have to be a little careful with the naming convention. It **has to be** the same as your github account name followed by *.github.io*
I made the mistake of not reading this instruction and tried to name my repository something else. The repository didn't link with my Github account and I'm not really sure where it ended up but moral is it didn't work.
Once I read the instructions properly and made the repository with my account name i.e bganko123.github.io all seemed to be working properly.
### Creating a nice homepage
To configure the blogs global settings I edited the *_config.yml* file. This allowed me to change the title and the description. Next I edited th markdown file *index.md*. This determines the contents of the homepage. I wrote a brief description that sums up the blog nicely
### Making posts
The first step is making a file with the correct name. **again** I didn't read the instructions at first and it definitely doesnt work if you don't follow them. The post file mut be named YEAR-MONTH-DAY-filename.md. The date allows the posts to be formatted into chronological order. 
Once you have the file setup and working correctly it is really just down to formatting. Below are some examples - for me to refer back to more than anything - of different ways to format
### Formatting options
For starters, you can control the font of the text. For example *italics*, **bold**, `code font`. You can add footnotes [^1] and horizontal lines

---

Next we have lists:
You can do dashes:
- x
- y
- z

or you can do numbers:

1. w
2. a
3. s
4. d

you can add quotes to make things stand out

> Taking a new step, uttering a new word, is what people fear most - Dostoesvky

Images are a little trickier. You first have to put the desired image into the image folder. An then you should be able to link it with the path and %![]% this command

![](/images/logo.png "fast.ai's logo")

## Code

General preformatted text:

    # Do a thing
    do_thing()

Python code and output:

```python
# Prints '2'
print(1+1)
```

    2

## Tables

| Column 1 | Column 2 |
|-|-|
| A thing | Another thing |

## Footnotes

[^1]: This is the footnote.
