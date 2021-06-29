# React Native App 
목적 : 
1. webview만으로 만드는 것이 아니라, native앱으로 만들고 싶어서 제작을 시도
2. 부분 webview를 도입해서 native 앱을 제작

사용하는 라이브러리 및 사용 방법
1. react native typescript 적용
```npm
   npm install --dev react-native-typescript-transformer typescript
   // react-native-typescript-transformer : 타입 스크립트를 읽어줄 수 있는 npm
   // typescript : typescript 적용
```
  - tsc-init 명령어를 통해서 해당하는 프로젝트의 tsconfig를 세팅
    - 만약 에러가 날 경우 global로 typescript가 선언이 안되어있어서 에러가 발생
      ```npm
        npm install -g typescript
      ```
  - 타입스크립트가 프로젝트 내에서 타입에 관한 리액트와 RN을 할 수 없어서
    ```npm
        npm install --dev @types/react @types/react-native
    // 프로젝트내에서 사용할 type react와 type react-native를 설치
    ```
  - typescirpt에서 테스트 코트를 작성하기
    ```npm
        npm install --dev ts-jest @types/jest
    ```

2. react native ui libray
  - ui-kitten
    - 다양한 ui와, 아이콘 등을 제공해서 우선적으로 사용
    - 안티와 이런것들보다 우선순위인 이유는 해당하는 제가 만들고싶은 ui를 제공을 해준다
    
3. react native Route
  - 네비게이터를 통해서 해당하는 페이지로 이동을 할 수 있고, 해당하는 페이지를 호출할 수 있다.
    ```npm
        npm install @react-navigation/native // 네이게이터의 초기 세팅
        npm install react-native-reanimated react-native-gesture-handler react-native-screens react-native-safe-area-context @react-native-community/masked-view
        npx pod-install ios // only ios
    ```
