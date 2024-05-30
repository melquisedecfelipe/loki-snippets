![loki-snippets](./logo/theme-icon.png)

# Loki Snippets for VS Code.

Loki is composed of a common snippets to use in [React](https://react.dev/) ecosystem.

# Installation

1. Open **Extensions** sidebar panel in VS Code. `View > Extensions`
2. Search for **`Loki Snippets`**
3. Click **Install** to install it

To use it, just type snippet and press `Enter`, when the snippet contains parameters just fill and navigate on next using `Tab`.

### EXAMPLES

We have several snippets and we'll be adding new ones over time, here's the list:

### React

`ir`: `import React from 'react'`

#### `rc`: Component

```tsx
import React from 'react'

export const Snippets = () => {
  return <div></div>
}

```

#### `rfc`: Function component

```tsx
import React from 'react'

export function Snippets() {
  return <div></div>
}

```

#### `rcp`: Component with props

```tsx
import React from 'react'

type SnippetsProps = {

}

export const Snippets = (_: SnippetsProps) => {
  return <div></div>
}

export default Snippets

```

#### `rfcp`: Function component with props

```tsx
import React from 'react'

type SnippetsProps = {
  foo: string
  bar: number
}

export const Snippets = (_: SnippetsProps) => {
  return <div></div>
}

export default Snippets

```

### React Testing Library

`irtl`: `import { cleanup, render } from '@testing-library/react'`

#### `rtld`: describe

```tsx
import { cleanup, render } from '@testing-library/react'

describe('Snippets', () => {
  afterEach(cleanup)

  it('should render correctly', () => {
    const { container } = render(<Snippets />)

    expect(container).toBeInTheDocument()
  })
})

```

#### `rtli`: it

```tsx
it('should render correctly', () => {
  const { container } = render(<Snippets />)

  expect(container).toBeInTheDocument()
})

```

#### `rtlie`: it.each

```tsx
const cases = [{ disabled: true, name: 'Snippets' }, { className: 'p-4' }]

it.each(cases)('should render correctly with props', props => {
  const { container } = render(<Snippets {...props} />)

  expect(container).toBeInTheDocument()
})

```

### Typescript

#### `tsa`: Arrow function

```ts
const snippets = () => {
  return
}

```

#### `tsf`: Function

```ts
function snippets() {
  return
}

```

#### `tst`: Type

```ts
type Snippets = {
  
}

```

#### `tsi`: Interface

```ts
interface Snippets {
  
}

```

Loki Snippets created by [Melquisedec Felipe](https://github.com/melquisedecfelipe).
