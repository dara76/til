Stateless function 

```
const NumberInput = ({min, max}) => {  
  return (  
    <span>  
      <input type="number" min={min} max={max} />  
    </span>
  }
}
```

becomes

```
class NumberInput extends Component {
  constructor(props) {
    super(props);
  }

  render () {
    const {min, max} = this.props;

    return (
      <span>
        <input type="number" min={min} max={max} />
      </span>
    );
  }
}
```

I can now use `ref` to focus on the input, which I couldn't in the stateless function above.

```
<input
  ref={input => input && input.focus()}
  //...
>
```

<https://facebook.github.io/react/docs/reusable-components.html#stateless-functions>
