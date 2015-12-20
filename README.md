# react-native-input
采用React Native开发,实现Input组件，支持往input中增加icon
![input输入框](https://github.com/chenchunyong/react-native-input/raw/master/input.png)

# Install
 
 安装包:
 
`npm i react-native-input --save`


通过引用`import Input from 'react-native-input'`来使用

# Demo

```
 React.createClass({
    render() {
        return (
            <InputText style={[{marginLeft:10,marginRight:10},this.props.style]}
                       keyboardType="numeric"
                       maxLength={11}
                       onChange={this.props.onChange}
                       placeholder={this.props.placeholder}
                       onFocus={this.props.onFocus}
                       onBlur={this.props.onBlur}
                       onGetContainerIcon={this._getPhoneNumIcon()}/>
        )
    },
    _getPhoneNumIcon(){
        return <Icon name="phone" style={s.icon}/>
    },
});
 
```

