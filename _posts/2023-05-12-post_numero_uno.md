# My first blog post - A blog post about blog posts
This is a brief overview of the things I learnt setting up my blog and making the first post

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
## Formatting options
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

Images are a little trickier. You first have to put the desired image into the image folder. And then you can link to the image name from that folder

For example, here is an image of my dog causing havoc at puppy preschool
![](/images/251013527_312706310369794_5735209258452722059_n.jpg "albert causing trouble")

Next we have code, there are a few ways to do it.
You can use just use a general preformatted version

    # do the thing
    do__the_thing()

Or alternatively you can use python specific code

```python
# Prints a number
print(8)
```

    8

Next we have tables. I find these a bit confusing because I don't really know what's what but here is an example anyway

| Column 1 | Column 2 |
|-|-|
| hello | Goodbye |

I'm sure there are a lot more things that can be done, but this seemed like a good start.

Ben

vvvvv Our foot note from above
[^1]: This is the footnote.
