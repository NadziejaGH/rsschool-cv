# **Nadzieja Konstanciuk**

### *Junior Frontend Developer*

🌟🌟🌟🌟🌟🌟🌟🌟🌟🌟🌟🌟

---

#### Contact information:  
* p96986967@gmail.com 
* [GitHub](https://github.com/NadziejaGH)   
* [LinkedIn](https://linkedin.com/in/nadziejagh)  

---
#### Summary

I am a beginner developer currently studying at RS School and working on small web projects.  
I enjoy tackling challenging tasks and learning new things every day.
I am passionate about coding, problem-solving, and continuous self-improvement.  
My goal is to become a full-stack developer and gain enough practical experience to start my career in IT.
I am motivated, fast-learning, and ready to grow as part of a development team.

---
#### Skills

* HTML5, CSS3 (Preprocessor SCSS, BEM methodology)
* JavaScript Basics
* Git, GitHub
* Figma(for web development)
* VS Code, WebStorm
* Vite, Minista

---
#### Code examples

This is a simple JavaScript-based random password generator.  
It creates a password using a predefined set of characters, including letters, numbers, and symbols.

The password is generated using the standard `Math.random()` function, which makes it suitable for basic use cases such as temporary or low-security passwords.

Note: This implementation does not use cryptographically secure random generation (e.g., `crypto.getRandomValues()`), so it is not recommended for sensitive data or high-security applications.

```
const buttonGenerate = document.querySelector('[data-js-generator-button]')
const inputPassword = document.querySelector('[data-js-generator-field__control]')
const copyPasswordIcon = document.querySelector('[data-js-generator-field__image]')
const alertMessage = document.querySelector('[data-js-alert-container]');

buttonGenerate.addEventListener('click', () => {
    createPassword()
});
copyPasswordIcon.addEventListener('click', () => {
    copyPassword();
    if (inputPassword.value){
        alertMessage.classList.remove('active');
        setTimeout(() => {
            alertMessage.classList.add('active')
        }, 3000);
    }
});
function createPassword() {
    const chars = '0123456789abcdefghijklmnopqrstuvwxtz!@#$%^&*()_+?:{}[]ABCDEFGHIJKLMNOPQRSTUVWXYZ';
    const passwordLength = 18;
    let password = "";
    for (let index = 0; index < passwordLength; index++) {
        const randomNum = Math.floor(Math.random() * chars.length);
        password += chars.substring(randomNum, randomNum + 1);
    }
    inputPassword.value = password;
    alertMessage.textContent = password + '\nHasło zostało skopiowane!';
}

function copyPassword() {
    inputPassword.select();
    inputPassword.setSelectionRange(0, 9999);
    navigator.clipboard.writeText(inputPassword.value);
} 
```
---
#### Education
* Rs-School. Statistics JS/FE Pre-School 2026 Q1 (in progress)

---
#### Languages:
1. English  - Elementary
2. Russian - Native
3. Polish - Intermediate


