Input-method is the blender of html input element. \
This case tells you why: [playground](https://cfdxkk.github.io/input-method-is-the-blender-of-html-input-box/)

[<img width="1903" height="400" alt="image" src="https://github.com/user-attachments/assets/d6a97440-4d3d-4c16-b7c6-8ee2d1e3bcca" />](https://cfdxkk.github.io/input-method-is-the-blender-of-html-input-box/)


<details> <summary>The culprit</summary>
  
  ```
    <input id="test-input" type="text" />

    ...

    document.querySelector("#test-input").addEventListener("input", toUppercase)
    function toUppercase(event) {
      event.target.value = event.target.value.toUpperCase()
    }
  ```

</details>
