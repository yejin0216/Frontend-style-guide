### CSS Naming Convention

- 변수명은 접두사에  `$`를 붙이고 *kebob-case*의 명사로 작성한다.

  - 좋은 예

  ```
  $font-color = #000000;
  ```
  
- `{Block}__{Element}--{modifier}` 순으로 작성한다. (*BEM* 참고)

  - 좋은 예
  
  ```
  .login__modal { //.. }
  .login__modal--active { //.. }
  ```  
  ```
  .nav__button { //.. }
  .nav__button--disable { //.. }
  ```
