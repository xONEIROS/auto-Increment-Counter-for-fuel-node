<div align="center">
    <h1>auto Increment Counter for fuel node</h1>
</div>

<div align="center">
    <p>
        <a href="README-fa.md">
            <small>فارسی</small>
            <img src='assets/ir.svg' alt='persian' style='width: 20px;height: 15px;border-radius: 3px;' />
        </a>
        | 
       <img src='assets/gb.svg' alt='English' style='width: 20px;height: 15px;border-radius: 3px;' />
        <small>English</small>
    </p>
</div>


![image](https://github.com/xONEIROS/auto-Increment-Counter-for-fuel-node/assets/174752031/ec41adf6-335e-4acd-b745-c90c4fd4c70a)

With this code, you can easily increase your Fuel node transactions. Just run this code in your browser's console, and it will automatically handle transactions as long as the console and your dapp window are open.

##Make sure you have a [faucet](https://faucet-beta-5.fuel.network/) ; otherwise, the transactions will fail.


To use this, you need to paste the code below into your browser's console (just copy and paste it). I recommend using the Brave browser.

1. First, open the link to your Fuel node Dapp.
2. Press F12 to open the console.
3. Paste the code and press Enter.
4. That's it! Let the transactions process automatically. You don't need to do anything else. You can minimize the browser and continue with your other tasks!

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

Keep in mind that in the parameter `setTimeout(clickButton, getRandomInterval(8, 13));` you can change the transaction timing.
However, it's recommended not to set it to less than 8 seconds to ensure the transactions go through. You can adjust this range as you prefer, for example: `(10, 20)`.

## [Telegram](https://t.me/xOneiros) | [Twitter](https://x.com/0xOneiros)

