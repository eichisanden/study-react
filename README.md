# study-react

Setup
----

```

```

JSX
----

## 属性

```javascript
var className = 'app';
<div className={className}></div>;
```

## Comment

```javascript
<div>
{/* Comment */}
<input
/*
 Comment
*/
name="name" // Comment
/>
</div>;
```
this.props.children

コンポーネント作成時の呼び出し順
getDefaultProps（２回目以降は呼ばれない）
getInitialState
componentWillMount
render
componentDidMount
  React.findDOMNode(this)でDOM要素にアクセス可能

コンポーネント作成後
componentWillReceiveProps
shouldComponentUpdate
  falseを返すと以後の３処理がスキップされる
componentWillUpdate
render
componentDidUpdate


コンポーネント破棄時
componentWillUnMount
