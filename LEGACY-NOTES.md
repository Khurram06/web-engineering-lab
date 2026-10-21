### Native Equivalents

- `$(document).ready` -> `type="module"` script, or `DOMContentLoaded` event
- `$("#name").val()` -> `document.querySelector("#name").value`
- `.after(html)` -> `element.after(newElement)`
- `$(".error").remove()` -> `document.querySelectorAll(".error").forEach(el => el.remove())`
- `.text(…).hide().fadeIn(400)` -> `element.textContent = …` followed by a CSS transition
- `$form[0].reset()` -> `formElement.reset()`

### Legacy Smells

- Using `var` instead of `const` or `let`
- Using `$.trim` instead of the native `.trim()` string method
- Using `.indexOf("@") === -1` instead of modern `.includes("@")`
- Building HTML elements by concatenating raw strings instead of `document.createElement`
