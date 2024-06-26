# React & Tailwind ToolBox

An opinionated React, NativeWind & Tailwind live template for IntelliJ products. <br/>
These live templates are created in the way I like to use in my daily work
flow, I prefer to have my types at the top of the file and I like to export
inline where I declare my component.

<br/>

### Where to put the template.xml

Rename the template to what ever you want to call it i.e. ```lukesReactToolBox.xml```
then drop the file into the following location:

``
/Users/yourUser/Library/Application\Support/JetBrains/WebStorm2023.3/templates/lukesReactToolBox.xml
``


<br/>
<br/>



[React Generic Shortcuts](#react-generic-shortcuts) |
[React Web Shortcuts](#react-web-shortcuts) |
[NativeWind Shortcuts](#native-wind-shortcuts) |
[Tailwind Shortcuts](#tailwind-shortcuts)

### React Generic Shortcuts

```uses```
Creates a useState with a null value

```tsx
const [state, setState] = useState(null)
```

```usee```
Creates a styled useEffect with no deps

```tsx
useEffect(() => {

}, [])
```

```af```
Creates a styled arrow function

```javascript
const handleSomething = () => {

};
```

<br/>

### React Web Shortcuts

```rfc```
Creates a simple Functional Component - Uses current filename without extension

```jsx
export default function FileName() {
    return (
    <div className={``}>
    
    </div>
    );
};
```

```rtfc```
Creates a Typed Functional Component - Uses current filename without extension

```tsx
import {FC} from "react";

interface FileNameProps {
  prop: string;
}

export const FileName: FC<FileNameProps> = ({prop}) => {

    return (
        <div className={``}>
            {prop}
        </div>
    );
};
```

```rtern```
Creates a styled ```TERNARY``` operation for ```<div>``` rendering with className

```tsx
{
    value ? (
        <div className={``}></div>
    ) : (
        <div className={``}></div>
    )
}
```

```rand```
Creates a styled ```AND``` operation for ```<div>``` rendering with className

```tsx
{
	value && (<div className={``}></div>)
}
```

<br/>

### Native Wind Shortcuts

```nwfc```
Creates a NativeWind Simple Functional Component - Uses current filename without extension

```tsx
import {View, Text} from "react-native";

export default function TestFile() {
    return (
        <View className={``}>
    
        </View>
    );
};
```

```nwtfc```
Creates a NativeWind Typed Functional Component - Uses current filename without extension

```tsx
import {FunctionComponent} from "react";
import {View, Text, ViewStyle} from "react-native";

interface OwnProps {
  style: ViewStyle;
}

type Props = OwnProps;

export const ComponentName: FunctionComponent<Props> = (props) => {
    const {style} = props
    
    return (
        <View style={style} className={``}>
    
        </View>
    );
};
```

```nwview```
Creates a styled NativeWind ```<View>``` with ClassName

```tsx
<View className={``}>

</View>
```

```nwtext```
Creates a styled NativeWind ```<Text>``` with ClassName

```tsx
<Text className={``}>

</Text>
```

```nwtern```
Creates a styled ```TERNARY``` operation for ```<View>``` rendering with className

```tsx
{
	value ? (
		<View className={``}></View>
	) : (
		<View className={``}></View>
	)
}
```

```nwand```
Creates a styled ```AND``` operation for ```<View>``` rendering with className

```tsx
{
	value && (<View className={``}></View>)
}
```

<br/>

### Tailwind Shortcuts

```twdiv```
Creates a styled div with flex

```tsx
<div className={`flex`}>

</div>
```

```twrow```
Creates a styled row

```tsx
<div className={`flex flex-row gap-4`}>

</div>
```

```twcol```
Creates a styled column

```tsx
<div className={`flex flex-col gap-4`}>

</div>
```

```twtern```
Creates an ```in line TERNARY``` operation for ```class``` styling based
on a ```value```

```tsx
${value ? "" : ""}
```

```twor```
Creates an ```in line OR``` operation for ```class``` styling based on a ```nullable
value```

```tsx
${value || ""}
```

```twand```
Creates an ```in line AND``` operation for ```class``` styling based on a ```value```

```tsx
${value && ""}
```




