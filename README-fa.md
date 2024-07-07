# افزایش خودکار شمارنده برای نود Fuel
![image](https://github.com/xONEIROS/auto-Increment-Counter-for-fuel-node/assets/174752031/ec41adf6-335e-4acd-b745-c90c4fd4c70a)

با این کد، می‌تونید به راحتی تراکنش‌های نود Fuel خودتون رو افزایش بدید. کافیه این کد رو توی کنسول مرورگرتون اجرا کنید و تا زمانی که کنسول و پنجره dapp شما باز باشه، تراکنش‌ها به صورت خودکار انجام می‌شه.

## دقت کنید که باید یه [faucet](https://faucet-beta-5.fuel.network/) داشته باشید؛ در غیر این صورت، تراکنش‌ها ناموفق خواهند بود.

برای استفاده، باید کد زیر رو توی کنسول مرورگر قرار بدید (کپی و پیست کنید). من مرورگر Brave رو پیشنهاد می‌کنم.

1. اول، لینک Dapp نود Fuel خودتون رو باز کنید.
2. کلید F12 رو بزنید تا وارد کنسول بشید.
3. کد رو قرار بدید و اینتر بزنید.
4. تمام! اجازه بدید تراکنش‌ها به صورت خودکار انجام بشن. نیاز نیست کار خاصی بکنید، می‌تونید مرورگر رو مینیمایز کنید و بقیه کارهاتون رو انجام بدید!

```
function getRandomInterval(min, max) {
    return Math.floor(Math.random() * (max - min + 1) + min) * 1000;
}

function clickButton() {
    var buttons = document.querySelectorAll('button');
    var button;
    for (var i = 0; i < buttons.length; i++) {
        if (buttons[i].innerText === "Increment Counter") {
            button = buttons[i];
            break;
        }
    }
    if (button) {
        button.click();
        console.log('Button clicked at ' + new Date().toLocaleTimeString());
    } else {
        console.log('Button not found');
    }
    setTimeout(clickButton, getRandomInterval(8, 13));
}

clickButton();
```

دقت داشته باشید که در پارامتر `setTimeout(clickButton, getRandomInterval(8, 13));` می‌تونید زمان انجام تراکنش رو تغییر بدید. اما پیشنهاد می‌کنیم که زمان رو کمتر از ۸ ثانیه نکنید تا تراکنش‌ها انجام بشن. می‌تونید این بازه رو مطابق میل خودتون تغییر بدید، مثلاً: `(10, 20)`.

## [تلگرام](https://t.me/xOneiros) | [توییتر](https://x.com0xOneiros)
