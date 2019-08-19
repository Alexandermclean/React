### 1.声明组件时用大写
```javascript
class Welcome2 extends React.Component {
  render () {
    return <h1>Hello, {this.props.name}</h1>
  }
}

const wel2 = <Welcome2 name='yuhui' />
```
> Welcome2 而不是 welcome2

### 2.同时引用组件用数组包含
```javascript
ReactDOM.render(
  [wel1, wel2], // 这里用数组
  document.getElementById('root')
);
```

### 3.渲染时组件标签的写法
```javascript
function Welcome1 (props) {
  return <h1>Hello, {props.name}</h1>;
}

function Noprop () {
  return <h1>yuhui</h1>
}

ReactDOM.render(
  [<Welcome1 />, <Noprop/>],
  document.getElementById('root')
)
```
