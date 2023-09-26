# Lukes' React & Tailwind ToolBox
An opinionated React & Tailwind live template for IntelliJ products. <br/>
These live templates are created in the way I like to use in my daily work
flow, I prefer to have my types at the top of the file and I like to export 
inline where I declare my component.

<br/>

[React Shortcuts](#react-shortcuts) |
[Tailwind Shortcuts](#tailwind-shortcuts)

### React Shortcuts
```rftc```
Creates a React Functional Typed Component
```typescript
import React from "react";

interface $ComponentName$Props {
  prop: string;
}

export const $ComponentName$: React.FC<$ComponentName$Props> = (props) => {
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




