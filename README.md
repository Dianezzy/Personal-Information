# 我的Resume

## How To Use?

### Compile

```
xelatex resume.tex % 编译英文简历
xelatex resume-zh_CN.tex % 编译中文简历
```

### Chinese fonts

中文模板与英文模板的区别仅有两行——使用中文时仅需反注释以下两行，模板中已默认启用，第一次编译时耗时相对较长(引入了外部中文字型)，耐心等待下。

```latex
\usepackage{zh_CN-fonts} % Simplified Chinese Support using system fonts
\usepackage{linespacing_fix} % disable extra space before next section
```

### Macro Definitions

- `\name`: 姓名
- `\contactInfo`: 联系信息, 需要三项信息，分别是{邮箱}{手机号}{个人主页} 最后一项可以为{}, 但不能去掉括号，否则编译不过
- `\section`: 用于分节, 如教育背景, 实习/项目经历等
- `\subsection`: 用于小节标题, 无日期选项
- `\datedsubsection`: 用于小节标题, 简历中使用最广，第二项为时间区间，自动右对齐
- `\itemize`: 清单列表，简历中应用最广
- `\enumerate`: 枚举列表，数字标号

### FontAwesome

首先在 [Font Awesome Icons](http://fortawesome.github.io/Font-Awesome/icons/) 上选中自己想使用的图标(暂不支持 alias)，然后在 [fontawesome.sty](https://github.com/billryan/resume/blob/zh_CN/fontawesome.sty) 中找到相应的宏, 将其作为普通文本一样使用。

## License

[The MIT License (MIT)](http://opensource.org/licenses/MIT)

Copyrighted fonts are not subjected to this License.
