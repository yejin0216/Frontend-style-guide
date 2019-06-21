### Vuejs Naming Convention

- 변수 이름은 *camelCase*의 명사로 작성한다.

  - 좋은 예

  ```
  let loginId; 
  let loginPwd; 
  ```

- 함수 이름은 *camelCase*의 동사로 작성한다.

  - 좋은 예
  
  ```
  const login = () => {
    //...
  }
  const getAccessToken = () => {
    //...
  }
  ```
  
- 상수는 대문자의 *Underscore Notation*로 작성한다. 

  - 좋은 예

  ```
  const LOGIN_ACCESS_TOKEN;
  ```

- root 컴포넌트인 ``App`` 컴포넌트를 제외한 컴포넌트 이름은 항상 합성어를 사용한다.

  - 좋은 예

  ```
  Vue.component('todo-item', {
    //...
  })
  ```

  ```
  export default {
    name: 'TodoItem'
  }
  ```

- 컴포넌트 이름(합성어)에 단어는 일반적인 단어와 수식하는 단어로 끝나야 한다. 

  - 좋은 예

  ```
  components / 
  | - SearchButtonClear.vue 
  | - SearchButtonRun.vue 
  | - SearchInputQuery.vue 
  | - SearchInputExcludeGlob.vue 
  | - SettingsCheckboxTerms.vue 
  | - SettingsCheckboxLaunchOnStartup.vue
  ```

- 컴포넌트 이름은 약어보다 완전한 단어가 좋다. 

  - 좋은 예

  ```
  components / 
  | - StudentDashboardSettings.vue 
  | - UserProfileOptions.vue
  ```

- 싱글 파일 컴포넌트의 이름은 *PascalCase* 나 *Kebob-case*로 한다.

  - 좋은 예

  ```
  components / 
  | - MyComponent.vue
  ```

  ```
  components / 
  | - my-component.vue
  ```

- 베이스 컴포넌트 이름은 특정 접두어로 시작해야한다. (Base, App, V 등)

  - 좋은 예

  ```
  components / 
  | - BaseButton.vue 
  | - BaseTable.vue 
  | - BaseIcon.vue
  ```

  ```
  components / 
  | - AppTable.vue 
  | - AppIcon.vue
  ```

  ```
  components / 
  | - VButton.vue 
  | - VTable.vue 
  | - VIcon.vue
  ```

- 연관성을 가진 컴포넌트일 경우 하위 컴포넌트의 이름은 상위 컴포넌트 이름을 접두사로 포함한다. 

  - 좋은 예

  ```
  components/
  | - TodoList.vue 
  | - TodoListItem.vue 
  | - TodoListItemButton.vue
  ```

- 플로그인, mixin 등에서 커스텀 사용자 private 프로퍼티에는 항상 접두사 ``$_``를 사용하고, 다른 사람의 코드와 충돌을 피하려면 named scope를 포함한다. 

  - 좋은 예 

  ```
  var myGreatMixin = {
    // ...
    methods: {
      $_myGreatMixin_update: function () {
        // ...
      }
    }
  }
  ```
