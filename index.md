Generic info about the webcomponent package.

## How to use

1. install

    ```
    npm install --save @hello
    ```

2. usage with preact/react
    
    ```typescript jsx
    
    declare global {
      namespace JSX {
        interface IntrinsicElements {
          ['hello']: CustomElement;
        }
      }
    }
    ...
    
    <hello />
    ```

3. usage with SSR (next.js)

    ```typescript jsx
       
    export const MyCustomComponent : FC = (props) => {
        return <hello>no WebComponent</hello>
    }
    ```

