# As you can see, this blog hasn't had a post since forever.

And I'm gonna explain why.

First of all, I'm only covering the technical aspect here; the personal reasons for the absence of written content have [their own post](//not-a-web-developer.srht.site/2022/June/writing.gmi) on my gemini capsule.

---

Ever since the beginning of this blog, I've written all the html and CSS by hand. This has had its advantages:
- i don't have to depend on a complicated build system, so i spend more time writing than fiddling with the ins and outs of said build system
- it's a bloody website for fuck's sake, why would I want to install half a million dependencies and write a ton of configuration files, templates and scripts just to output text on a screen? It feels wrong.
- forget about feelings, who cares if it works, right? But it doesn't work; at least for me, every SSG i tried i couldn't wrap my head around how it worked and how to use it.

## okay, i guess it's time for a list of all the SSGs i tried:

1. [Jekyll](http://jekyllrb.com/);
2. [11ty](https://www.11ty.dev/);
3. [Hugo](https://gohugo.io/);
4. [Franklin.jl](https://franklinjl.org/) (yes, i tried Julia too, that will get its own ~~rant~~ blogpost later); and last but not least
5. [Gatsby](https://www.gatsbyjs.com/)

The problem with these wasn't the fact that they don't work at all; I mean, people use these tools daily and make some [really](https://github.com/jeffreytse/jekyll-theme-yat/) [beautiful](https://github.com/yinkakun/eleventy-duo) [themes](https://themes.gohugo.io/themes/hermit/) for them.

### I don't want to use their themes. I want the website to stay the same, visually.

That means I need to be able to figure out how to port over my website to one of these SSGs, since I'm not spending the time to rebuild my website from scratch just to have it fit one of them. That might sound lazy, and it is; however, you'll soon understand why.

## So, how did they fare?

in short? not well.

longer explanation? Well, here's a breakdown:

1. Jekyll: Since Github Pages, on which the website is currently hosted, is built in Jekyll, it should be the best option; however, I wasn't able to understand how to import a custom css file for Jekyll. As far as I can see, the only way to get custom styling in jekyll is to make my own theme, host it on Github, and reference it in the `_config.yml` like this:
```yaml
remote_theme: "not-a-web-developer/my-jekyll-theme"
```
making an entire jekyll theme by myself is too much for me to be able to do, so that's one option down.

2. 11ty: same problem as Jekyll, the website was really complicated for me to navigate through, and i couldn't figure out how to get CSS working, or even what to write in; long story short, it was choice paralysis and the explanations for all the options went over my head, which didn't help.

3. Hugo: Hugo also apparently requires you to choose a theme, and making a theme requires knowing Go; which unfortunately makes it a no-go for me, since i'm not quite interested (nor have the mental capacity) in learning Go at the moment. <br>
\<tangent\><br>
I understand that I can abuse the static files directory ([this](https://gohugo.io/content-management/static-files/)) to store my css, but this is just a workaround and i do not expect it to work at all.<br>
\</tangent\>

4. 
