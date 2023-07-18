# from JS to React

## **React Core Concepts**

- Components
- Props
- State

untuk berpindah antara JSX ke JS => () dan {}
- () => didalamnya berisi syntax JSX
- {} => didalamnya berisi syntax JS

### Components

di React **Components** merupakan sebuah **function** yang mengembalikan sebuah **Element UI**

untuk membuat **Components** bekerja, ada dua hal yang harus dilakukan :

1. _React Components_ harus di **capitalized** (penulisan kata di huruf pertama nya harus huruf besar) untuk membedakan untuk membedakan antara HTML biasa dengan Javascript.

```jsx
function Header(){
      return (<>
        <h1>Learn From JavaScript to React</h1>
        <h2>By NextJS Tutorial</h2>
      </>)
    }
```

2. ketika menggunakan _React Components_ sama seperti ketika menggunakan tag HTML biasa, dengan menggunakan tanda `</>`

```jsx
ReactDOM.render(<HomePage />,app)
```

#### Nesting **Components**

aplikasi biasanya berisi lebih banyak kontent daripada satu components.

```jsx
function Header(){
      return (<>
        <h1>Learn From JavaScript to React</h1>
        <h2>By NextJS Tutorial</h2>
      </>)
    }

function HomePage(){
      return (<>
    {/* nesting the Header Components*/}
    <Header/>
    <p>Hello I'M fani alfirdaus</p>
      </>)
    }
```

dengan begitu, kamu dapat nesting react component seperti ini untuk membuat pohon components.