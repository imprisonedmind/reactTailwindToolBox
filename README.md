# Lukes' React & Tailwind ToolBox
An opinionated React & Tailwind live template for IntelliJ products. <br/>
These live templates are created in the way I like to use in my daily work
flow, I prefer to have my types at the top of the file and I like to export 
inline where I declare my component. 

[React Shortcuts](#react-shortcuts)
[Tailwind Shortcuts](#tailwind-shortcuts)

<br/>

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

<br/>

```uses```
Creates a useState with a null value
```typescript
const [state, setState] = useState(null)
```

<br/>

```usee```
Creates a styled useEffect with no deps
```typescript
useEffect(() => {
    
},[])
```

<br/>

```af```
Creates a styled arrow function
```typescript
const handleSomething = () => {

};
```

<br/>

### Tailwind Shortcuts
```div```
Creates a styled div with flex
```tsx
<div className={`flex`}>

</div>
```

<br/>

```row```
Creates a styled row
```tsx
<div className={`flex flex-row gap-4`}>

</div>
```

<br/>

```col```
Creates a styled column
```tsx
<div className={`flex flex-col gap-4`}>

</div>
```




