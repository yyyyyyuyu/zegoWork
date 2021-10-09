## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/yyyyyyuyu/zegoWork/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

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

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/yyyyyyuyu/zegoWork/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.


### vue-cli4  + vue3.0  On-demand Import  element-plus


[Link]https://github.com/element-plus/unplugin-element-plus    按需引入样式

[Link]https://github.com/antfu/unplugin-vue-components#readme  按需引入组件


### vue.config.js
```markdown
const {ElementPlusResolver }= require('unplugin-vue-components/resolvers')

module.exports = {
  configureWebpack: {
    plugins: [
      require('unplugin-vue-components/webpack')({
        resolvers: [ElementPlusResolver()],
        dts: true,
        include: [/\.vue$/, /\.vue\?vue/, /\.md$/],
      }),
      require('unplugin-element-plus/webpack')({
        resolvers: [ElementPlusResolver()],
        dts: true,
        include: [/\.vue$/, /\.vue\?vue/, /\.md$/],
      }),
    ],
  },
}

```
# some errors : "export 'createElementBlock' was not found in 'vue'
resolution 1:  update vue3.0.0 to the latest version (vue3.2.0 2021/10/9)



