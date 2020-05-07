# React-Pokemon

## Notes

- `yarn add @apollo/react-hooks`
- `yarn add apollo-boost`
- `yarn add graphql`

> `https://graphql-pokemon.now.sh/`

### 初始化 ApolloClient

```js
import ApolloClient from 'apollo-boost';
import { ApolloProvider } from '@apollo/react-hooks';

function App() {
  const client = new ApolloClient({
    uri: 'https://graphql-pokemon.now.sh',
  });

  return (
    <ApolloProvider client={client}>
      <main>
        <p>i am a Pokemon!</p>
      </main>
    </ApolloProvider>
  )
}
```
