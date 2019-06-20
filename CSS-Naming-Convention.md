### CSS Naming Convention

- index.scss에서 import 대상인 모든 scss의 파일명은 `_`로 시작하는 소문자 명사이다.

  - 좋은 예

  ```
  _auth.scss
  _variables.scss
  ```

- 변수명은 접두사에  `$`를 붙이고 *kebob-case*의 소문자 명사이다.

  - 좋은 예

  ```
  $font-color = #000000;
  ```
  
- `{Block}__{Element}--{modifier}` 순이며 소문자이다. (*BEM* 참고)

  - 좋은 예
  
  ```
  .login__modal { //.. }
  .login__modal--active { //.. }
  ```  
  ```
  .nav__button { //.. }
  .nav__button--disable { //.. }
  ```
