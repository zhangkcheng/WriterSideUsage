# 主页

## 关于%product%

%product%是一个基于[IntelliJ Platform](https://www.jetbrains.com/opensource/idea/)的JetBrains IDE。
用于编写、构建、测试和发布技术文档。

这里是%product%的官方[技术文档](https://www.jetbrains.com/help/writerside/discover-writerside.html)。

## 文档目录

- [项目](project.md)
  - [实例类型](instances.md)
- 主题
- 标记文本
  - Semantic Markup Reference **语义标记参考**
  - Paragraphs **段落**
  - Structural Elements **结构元素**
  - Collapsible Elements **可折叠元素**
  - Links and References **链接和参照**
  - Images **图片**
  - Videos **视频**
  - Lists **列表**
  - Tables **表格**
  - Tabs **标签**
  - Code **代码**
  - Shortcuts **快捷键**
  - Tooltips **工具提示**
  - Admonitions **警告**
  - TLDR blocks **摘要**
  - Summary Elements **总结元素**
  - Starting Pages **起始页**
  - Downloadable Resources **可下载资源**
  - Mermaid Diagrams **Mermaid图表**
  - PlantUML Diagrams **PlantUML图表**
  - D2 diagrams **D2图表**
  - Math Expressions **数学公式**
  - API Documentation **API文档**
- 资源复用
- 预览和测试
- 构建和发布
- 自定义输出
- 导出PDF
- 其他

# About Index

<!--Writerside adds this topic when you create a new documentation project.
You can use it as a sandbox to play with Writerside features, and remove it from the TOC when you don't need it anymore.-->

## Add new topics
You can create empty topics, or choose a template for different types of content that contains some boilerplate structure to help you get started:

![Create new topic options](new_topic_options.png){ width=290 }{border-effect=line}

## Write content
%product% supports two types of markup: Markdown and XML.
When you create a new help article, you can choose between two topic types, but this doesn't mean you have to stick to a single format.
You can author content in Markdown and extend it with semantic attributes or inject entire XML elements.

## Inject XML
For example, this is how you inject a procedure:

<procedure title="Inject a procedure" id="inject-a-procedure">
    <step>
        <p>Start typing and select a procedure type from the completion suggestions:</p>
        <img src="completion_procedure.png" alt="completion suggestions for procedure" border-effect="line"/>
    </step>
    <step>
        <p>Press <shortcut>Tab</shortcut> or <shortcut>Enter</shortcut> to insert the markup.</p>
    </step>
</procedure>

## Add interactive elements

### Tabs
To add switchable content, you can make use of tabs (inject them by starting to type `tab` on a new line):

<tabs>
    <tab title="Markdown">
        <code-block lang="plain text">![Alt Text](new_topic_options.png){ width=450 }</code-block>
    </tab>
    <tab title="Semantic markup">
        <code-block lang="xml">
            <![CDATA[<img src="new_topic_options.png" alt="Alt text" width="450px"/>]]></code-block>
    </tab>
</tabs>

### Collapsible blocks
Apart from injecting entire XML elements, you can use attributes to configure the behavior of certain elements.
For example, you can collapse a chapter that contains non-essential information:

#### Supplementary info {collapsible="true"}
Content under a collapsible header will be collapsed by default,
but you can modify the behavior by adding the following attribute:
`default-state="expanded"`

### Convert selection to XML
If you need to extend an element with more functions, you can convert selected content from Markdown to semantic markup.
For example, if you want to merge cells in a table, it's much easier to convert it to XML than do this in Markdown.
Position the caret anywhere in the table and press <shortcut>Alt+Enter</shortcut>:

<img src="convert_table_to_xml.png" alt="Convert table to XML" width="706" border-effect="line"/>

## Feedback and support
Please report any issues, usability improvements, or feature requests to our
<a href="https://youtrack.jetbrains.com/newIssue?project=WRS">YouTrack project</a>
(you will need to register).

You are welcome to join our
<a href="https://jb.gg/WRS_Slack">public Slack workspace</a>.
Before you do, please read our [Code of conduct](https://plugins.jetbrains.com/plugin/20158-writerside/docs/writerside-code-of-conduct.html).
We assume that you’ve read and acknowledged it before joining.

You can also always email us at [writerside@jetbrains.com](mailto:writerside@jetbrains.com).

<seealso>
    <category ref="wrs">
        <a href="https://plugins.jetbrains.com/plugin/20158-writerside/docs/markup-reference.html">Markup reference</a>
        <a href="https://plugins.jetbrains.com/plugin/20158-writerside/docs/manage-table-of-contents.html">Reorder topics in the TOC</a>
        <a href="https://plugins.jetbrains.com/plugin/20158-writerside/docs/local-build.html">Build and publish</a>
        <a href="https://plugins.jetbrains.com/plugin/20158-writerside/docs/configure-search.html">Configure Search</a>
    </category>
</seealso>