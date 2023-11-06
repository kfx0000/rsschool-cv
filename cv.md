# Andrei Stupakou

## Contacts
* **E-mail:** kfx0000@gmail.com
* **Telegram:** @andySt
* **Discord:** Andrei Stupakou#0876
* **[GitHub](https://github.com/kfx0000)**

## Brief information about myself

I work as a lead network engineer. At now I guess I have reached my limits in this work. So, I want to change my major and learn JavaScript.

## Skills

As a Developer
* C/C++
* HTML
* CSS
* JavaScript (Fundamentals)

As an Engineer
* Networking (Cisco / HP)
* Microcontrollers (AVR / STM32)
* Hardware development (Altera)
* VoIP (Asterisk / FreeSwitch)

## Code example

DESCRIPTION:
>Implement function `check(str, bracketsConfig)`, that for given brackets sequence will return `true` if it is correct and `false` otherwise. <br>
> In the second param there is `bracketsConfig` - the array of pairs open-closed brackets. Each subarray includes only 2 elements - opening and closing bracket

SOLUTION:
```js
function check(str, bracketsConfig) {
  function removeInternal(arr) {
    for (let count = 0; count <= arr.length; count++) {
      for (let confPointer = 0; confPointer < bracketsConfig.length; confPointer++) {
        if ((arr[count] === bracketsConfig[confPointer][0]) && (arr[count + 1] === bracketsConfig[confPointer][1])) {
          arr.splice(count, 2);
          removeInternal(arr);
        }
      }
    }
    if (arr.length === 0) return true; else return false;
  }

  return removeInternal(str.split(''));
}
```

## Education
* **Udemy**
    * [HTML/CSS](https://www.udemy.com/course/webdeveloper/)
* **Rolling Scopes School**
    * [RS School JS/FE Pre-School 2023Q2](https://app.rs.school/certificate/z7cns0m5)

## Languages

* **Russian** - native
* **Belarussian** - native
* **English** - A2
