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



## Markdown

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


