---
title: 欢迎来到 Docusaurus v2
description: 这是我关于 Docusaurus 2 的第一篇博文。
slug: welcome-docusaurus-v2
image: https://i.imgur.com/mErPwqL.png
hide_table_of_contents: false
---

> 易于维护开源文档网站。
>
> — Docusaurus

这些都会变成博文摘要。

甚至包括这一行。

<!--truncate-->

但这一行和这一行下面的内容就不会了。

这行不会。

这行也不会。

### Details 元素示例

<details>
  <summary>点我！</summary>
  <div>
    <div>这是详情内容</div>
    <br/>
    <details>
      <summary>
        嵌套的下拉栏！ 内含惊喜……
      </summary>
      <div>
        😲😲😲😲😲
      </div>
    </details>
  </div>
</details>

export const Highlight = ({children, color}) => (
  <span
    style={{
      backgroundColor: color,
      borderRadius: '2px',
      color: '#fff',
      padding: '0.2rem',
    }}>
    {children}
  </span>
);

<Highlight color="#25c2a0">Docusaurus 绿</Highlight> 和 <Highlight color="#1877F2">Facebook 蓝</Highlight> 是我最喜欢的颜色。

我可以把我的 _JSX_ 和 **Markdown** 写在一起！

- 一个
- 列表！

和一些 <Highlight color="#25c2a0">自定义标记</Highlight>……


```jsx
/**
 * Copyright (c) Facebook, Inc. and its affiliates.
 *
 * This source code is licensed under the MIT license found in the
 * LICENSE file in the root directory of this source tree.
 */

import React, {useState} from 'react';

export default function MyComponent() {
  const [bool, setBool] = useState(false);
  return (
    <div>
      <p>MyComponent rendered !</p>
      <p>bool={bool ? 'true' : 'false'}</p>
      <p>
        <button onClick={() => setBool((b) => !b)}>toggle bool</button>
      </p>
    </div>
  );
}
```

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
  <TabItem value="apple" label="苹果" default>
    这是个苹果 🍎
  </TabItem>
  <TabItem value="orange" label="橙子">
    这是个橙子 🍊
  </TabItem>
  <TabItem value="banana" label="香蕉">
    这是个香蕉 🍌
  </TabItem>
</Tabs>

<Tabs groupId="operating-systems">
  <TabItem value="win" label="Windows">用 Ctrl + C 复制。</TabItem>
  <TabItem value="mac" label="macOS">用 Command + C 复制。</TabItem>
</Tabs>

<Tabs groupId="operating-systems">
  <TabItem value="win" label="Windows">用 Ctrl + V 粘贴。</TabItem>
  <TabItem value="mac" label="macOS">用 Command + V 粘贴。</TabItem>
</Tabs>

```jsx title="/src/components/HelloCodeTitle.js"
function HelloCodeTitle(props) {
  return <h1>你好，{props.name}</h1>;
}
```

```js
function HighlightSomeText(highlight) {
  if (highlight) {
    // highlight-next-line
    return '这行被高亮了！';
  }

  return '这里不会';
}

function HighlightMoreText(highlight) {
  // highlight-start
  if (highlight) {
    return '这块被高亮了！';
  }
  // highlight-end

  return '这里不会';
}
```

<pre>
  <b>输入：</b>1 2 3 4{'\n'}
  <b>输出：</b>"366300745"{'\n'}
</pre>

:::note

Some **content** with _Markdown_ `syntax`. 看看[这个 `api`](#)。

:::  

:::tip

Some **content** with _Markdown_ `syntax`. 看看[这个 `api`](#)。

:::  

:::info

Some **content** with _Markdown_ `syntax`. 看看[这个 `api`](#)。

:::  

:::caution

Some **content** with _Markdown_ `syntax`. 看看[这个 `api`](#)。

:::  

:::danger

Some **content** with _Markdown_ `syntax`. 看看[这个 `api`](#)。

:::  

<!-- Prettier doesn't change this -->
:::note

Hello world

:::  

<!-- Prettier changes this -->
:::note
Hello world
:::  

<!-- to this -->
::: note

Hello world

:::  

:::note Your Title

Some **content** with _Markdown_ `syntax`.

:::  

[链接](#heading-id)

<Link to="#heading-id">链接</Link>

### Hello World {#my-explicit-id}

# 你的文档
/website/docs/myFeature.mdx

# 你想用的一些静态资源
/website/docs/assets/docusaurus-asset-example-banner.png
/website/docs/assets/docusaurus-asset-example.docx

---
description：这段描述会覆盖默认值。
---

# 标题

主要内容…… 还可能包含一些链接或者**重点**。
