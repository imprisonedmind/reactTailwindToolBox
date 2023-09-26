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
```fc```
Creates a simple Functional Component - Uses current filename without extension
```javascript
export default function FileName() {
  return (
    <div className={``}>

    </div>
  );
};
```
```tfc```
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
```nwtfc```
Creates a NativeWind Typed Functional Component - Uses current filename without extension
```typescript jsx
import {FunctionComponent} from "react";
import {View} from "react-native";

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
```div```
Creates a styled div with flex
```tsx
<div className={`flex`}>

</div>
```
```row```
Creates a styled row
```tsx
<div className={`flex flex-row gap-4`}>

</div>
```
```col```
Creates a styled column
```tsx
<div className={`flex flex-col gap-4`}>

</div>
```




