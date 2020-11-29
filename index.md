## Appendix

### Other Experiments:

L2 Objective for GAN:

`loss_D = 0.5 * (tf.reduce_mean((outReal-1)**2)+tf.reduce_mean(outComp**2))`

`loss_GP = 0.5 * (tf.reduce_mean(outComp-1)**2)`


### Loss Plot

<img src="img/curve1.png" width=500>
<img src="img/curve2.png" width=500>
<img src="img/i1.png" width=500>
<img src="img/i2.png" width=500>

G produces parameters so that a major part of the bag is out of frame. It learned a trivial solution, when using the L2 loss.

## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/TensorHeads/tensorheads.github.io/edit/main/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/TensorHeads/tensorheads.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
