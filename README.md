Microsoft Pinyin is the blender of html input element. \
This case tells you why: [demo](https://cfdxkk.github.io/microsoft-pinyin-is-the-blender-of-html-input-element/)

<img width="696" height="135" alt="image" src="https://github.com/user-attachments/assets/f7cd7f42-5ab0-43fa-a428-7905cd69ed56" />

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
