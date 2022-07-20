### Ignite Lab 03
### especialização em React Native


https://efficient-sloth-d85.notion.site/Ignite-Lab-03-606aca4553fc4acc90505eae21521403

Instalando Expo:

Precisa saber se a versão do node Node v16.13.0 (LTS) esta instalada.
Caso não segui o caminho:
https://nodejs.org/ru/blog/release/v16.13.0/

Windows 64-bit Installer: https://nodejs.org/dist/v16.13.0/node-v16.13.0-x64.msi


`yarn global add expo-cli`

Para verificar se a instalação ocorreu com sucesso, execute o comando abaixo:

`expo --version`

No terminal do `git bash`, sera nescessario o argumento no modo não interativo:

`expo init rockethelp --template bare-minimum`

Agora no projeto vamos passa para TypeScript:
1 Vamos pegar o arquivo `App.js` e mudar a extenção dele para `tsx`.
2 Agora vamos criar um novo arquivo na raiz do projeto chamado `tsconfig.json` que ver ser um arquivo que o TypeScript usa para suas configurações.
3 inicia o projeto com expo, com o `expo start`

? It looks like you're trying to use TypeScript but don't have the required dependencies installed. Would you like to install typescript, @types/react,
@types/react-native? » (Y/n) = Y

<h1 align="center">
    <img src="./img/img000.png" />
</h1>
Para abilitar e desabilitar:
shift+d │ toggle auto opening developer tools on startup (disabled)

Para rodar o projeto no emulador:
Press a │ open Android

Pode precisar instalar:
https://developer.android.com/studio?hl=pt

Ou 

`› Press w │ open web`

Ou você pode instalar o APP no celular chamado `Expo Go`.

Dentro da pasta src/screens vamos criar o arquivo `SignIn.tsx`

E dentro vamos criar uma função e exporta ela para usar em outro arquivo como componente:

```
import { View, Text} from 'react-native';

export function SignIn(){
  return(
    <View>
      <Text>Olá, Marcelo</Text>
    </View>
  )
}
```

E no arquivo `App.tsx`:

```
import { SignIn } from './src/screens/SignIn'

export default function App() {
  return (
    <SignIn />
  );
}
```
A documentação da Native Base tem uma serie de componentes prontos para usar.

`https://nativebase.io/`

Vamos instalar o `yarn add native-base`.

Vamos instalar o `expo install react-native-svg`.

Vamos instalar o `expo install react-native-safe-area-context`.

E para usar o Native Base precisa envolver toda a aplicação
No arquivo `App.tsx` vamos fazer as seguinte configurações.

Baixa a pasta com as corres
https://efficient-sloth-d85.notion.site/Aula-02-95e894d266d84a0ca6e6604528cc12e3

Agora no arquivo `App.tsx` vamos fazer a importação do tema:

SVG transform react-native
Vai permiti que seja usado o SVG em forma de componente

https://github.com/kristerkari/react-native-svg-transformer

`yarn add --dev react-native-svg-transformer`

configurar o empacotador nativo do react
Para Expo SDK v41.0.0 ou mais recente
Mescle o conteúdo do metro.config.jsarquivo do seu projeto com esta configuração (crie o arquivo se ele ainda não existir).

`expo start --clear`

https://reactnavigation.org/docs/getting-started/

yarn add @react-navigation/native

expo install react-native-screens react-native-safe-area-context

yarn add @react-navigation/native-stack

## Integração com Firebase e finalização
