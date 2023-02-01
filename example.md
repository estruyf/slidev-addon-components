---
layout: default
colorSchema: dark
---

# Available components

- `box`: A simple box/rectangle component.
- `oval`: A simple oval/circle component.
- `show-hide`: A component which can be used to show and hide content.

---

# `box`

A simple box component.

```jsx
<box 
  left="400px" // required
  top="350px" // required 
  width="330px" // default: 100px
  height="100px" // default: 100px  
  borderColor="#44FFD2" // default: #fff 
  borderWidth="2px" // default: 2px
  borderStyle="solid" // default: solid 
  backgroundColor="#44ffd233" // optional 
  textColor="#fff" // default: inherit 
  title="Title" // optional 
  description="Description" // optional 
  />
```

<box 
  left="50px" 
  top="400px" 
  width="330px" 
  height="100px" 
  borderColor="#44FFD2" 
  borderWidth="5px" 
  borderStyle="solid" />


<box 
  left="400px" 
  top="400px" 
  width="330px" 
  height="100px" 
  borderColor="#44FFD2" 
  borderWidth="5px" 
  borderStyle="solid"
  backgroundColor="#44ffd233"
  textColor="#fff"
  title="Title"
  description="Description" />

---

# `oval`

A simple oval/circle component.

```jsx
<oval 
  left="400px" // required
  top="350px" // required 
  width="330px" // default: 100px
  height="100px" // default: 100px  
  borderColor="#44FFD2" // default: #fff 
  borderWidth="2px" // default: 2px
  borderStyle="solid" // default: solid 
  backgroundColor="#44ffd233" // optional 
  textColor="#fff" // default: inherit 
  title="Title" // optional 
  description="Description" // optional 
  />
```

<oval 
  left="50px" 
  top="400px" 
  height="100px" 
  borderColor="#44FFD2" 
  borderWidth="5px" 
  borderStyle="solid" />


<oval 
  left="400px" 
  top="400px" 
  width="330px" 
  height="100px" 
  borderColor="#44FFD2" 
  borderWidth="5px" 
  borderStyle="solid"
  backgroundColor="#44ffd233"
  textColor="#fff"
  title="Title"
  description="Description" />


---
clicks: 3
---

# `show-hide`

A component which can be used to show and hide content.

```jsx
---
clicks: 3 // Define the click count
---

<show-hide show="1" hide="2">
  Show on click 1, hide on 2, Current: {{ $slidev.nav.clicks }}
</show-hide>
```

<br />

<show-hide show="0" hide="1">
  Hide on 1, Current: {{ $slidev.nav.clicks }}
</show-hide>

<show-hide show="1" hide="2">
  Show on click 1, hide on 2, Current: {{ $slidev.nav.clicks }}
</show-hide>

<show-hide show="2" hide="3">
  Show on click 1, hide on 2, Current: {{ $slidev.nav.clicks }}
</show-hide>

