To apply css on dynamic class created by prime-ng we can use this  **::ng-deep** before classs selector

```css

::ng-deep .p-autocomplete-multiple-container {
  border-bottom: 1px solid #e9e9e9 !important;
  width: 100%;
  padding: 0 0.5rem;
}

::ng-deep .p-autocomplete-multiple-container .p-autocomplete-token {
  background-color: #fff !important;
  border: 1px solid #dadce0;
  border-radius: 15px !important;
  height: 1.5rem;
  line-height: 20px;
  padding-right: 4px !important;
  position: relative;
}

::ng-deep .p-autocomplete-input-token input[type="text"] {
  border-bottom: none !important ;
}

```
