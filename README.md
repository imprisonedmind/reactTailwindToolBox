# Luke's React & Tailwind ToolBox
An opinionated React & Tailwind live template for IntelliJ products. <br/>
These live templates are created in the way I like to use in my daily work
flow, I prefer to have my types at the top of the file and I like to export 
inline where I declare my component.

<br/>

[React Shortcuts](#react-shortcuts) |
[NativeWind Shortcuts](#native-wind-shortcuts) |
[Tailwind Shortcuts](#tailwind-shortcuts)

### React Shortcuts
```rfc```
Creates a simple Functional Component - Uses current filename without extension
```javascript
export default function FileName() {
  return (
    <div className={``}>

    </div>
  );
};
```
```rtfc```
Creates a Functional Typed Component - Uses current filename without extension
```typescript jsx
import {FC} from "react";

interface FileNameProps {
	prop: string;
}

export const FileName: FC<FileNameProps> = (props) => {
  const { prop } = props;

  return (
    <div className={``}>

    </div>
  );
};
```
```uses```
Creates a useState with a null value
```typescript
const [state, setState] = useState(null)
```
```usee```
Creates a styled useEffect with no deps
```typescript
useEffect(() => {
    
},[])
```
```af```
Creates a styled arrow function
```typescript
const handleSomething = () => {

};
```
```turn```
Creates a styled ```TERNARY``` operation for ```<div>``` rendering
```tsx
{value ? (
  <div className={``}></div>
) : (
  <div className={``}></div>
)}
```
```and```
Creates a styled ```AND``` operation for ```<div>``` rendering
```tsx
{value && (<div className={``}></div>)}
```

<br/>

### Native Wind Shortcuts
```nwfc```
Creates a NativeWind Simple Functional Component - Uses current filename without extension
```javascript jsx
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
```typescript jsx
import {FunctionComponent} from "react";
import {View, Text} from "react-native";

interface OwnProps {
  prop: string;
}

type Props = OwnProps;

export const ComponentName: FunctionComponent<Props> = (props) => {
  const {prop} = props

  return (
    <View className={``}>

    </View>
  );
};
```
```nwview```
Creates a styled NativeWind ```<View>``` with ClassName
```typescript jsx
<View className={``}>

</View>
```
```nwtext```
Creates a styled NativeWind ```<Text>``` with ClassName
```typescript jsx
<Text className={``}>

</Text>
```

<br/>

### Tailwind Shortcuts
```ilt```
Creates an ```in line TERNARY``` operation for ```class``` styling based 
on a ```value```
```tsx
${value ? "" : ""}
```
```ilor```
Creates an ```in line OR``` operation for ```class``` styling based on a ```nullable 
value```
```tsx
${value || ""}
```
```ila```
Creates an ```in line AND``` operation for ```class``` styling based on a ```value```
```tsx
${value && ""}
```
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




