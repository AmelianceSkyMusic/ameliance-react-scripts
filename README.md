# Ameliance SkyMusic React TypeScript Scripts Collection

A collection of my personal scripts, scripts I found on the Internet, maybe even modified

## Installation

```
npm i ameliance-react-scripts
```

## Usage

Import like this

```ts
import { splitTextByBr } from "ameliance-react-scripts";
```

or

```ts
import ars from "ameliance-react-scripts";

const randomRGBColor = ars.getRandomRGBColor();
```

## Functions list

### react

```ts
react.splitTextByBr('Hello!\nYour code is awesome!');

Hello!
<br />
Your code is awesome!

react.splitTextByBr("Some\nfew\nlines");
// <>
// 	some
// 	<br/>
// 	few
// 	<br/>
// 	lines
// 	<br/>
// </>
```

```ts
const isActiveClass = useActiveClass("some-class another-class");

function SomeComponent() {
	return <Link className={isActiveClass(link.path === path)} />;
}
```

### next

```ts
return next.api.generateResponseJsonError({
	status: 401,
	statusText: "Session is invalid",
	code: "SESSION_IS_INVALID",
});
```

```ts
return next.api.generateResponseJsonSuccess({ userId: 1234567890 });
```

## History

```
0.0.101 [2024_11_21]:
   +: add useActiveClass

0.0.1 [2024_11_19]:
   +: add splitTextByBr
   +: add generateResponseJsonError
   +: add generateResponseJsonSuccess
```
