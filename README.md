[![Linkedin: zarifpour](https://img.shields.io/badge/-zarifpour-blue?style=flat&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/zarifpour/)](https://www.linkedin.com/in/zarifpour/)
![](https://visitor-badge.glitch.me/badge?page_id=zarifpour.zarifpour)
<a href="https://zarif.pro/?ref=ghrdme" target="_blank"><img src="https://github.com/zarifpour/assets/blob/main/gifs/imposter.gif?raw=true" alt="imposter" width="75"></a>
<!-- <a href="https://www.buymeacoffee.com/zarifpour" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-red.png" alt="Buy Me A Coffee" width="150" ></a> -->

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.14;

import "@openzeppole/contracts/adjectives/Delicious.sol";

contract README is Delicious {
    address private owner;
    string public name;
    Emoji[] public skills;
    
    event Thank(address indexed sender);

    constructor() {
        owner = 0x5cfb84bf312f138129006500Bfb1606130640EDE;
        name = "Daniel Zarifpour";
        skills = ["💠", "🐍", "🔎", "🔒", "🧪", "🗣", "🎨"];
    }

    function donate() public payable {
        require(msg.value > 0, "That's not nice");
        require(msg.value < 1000000, "That's too nice");
        emit Thank(msg.sender);
    }
    
    function withdraw() external payable {
        require(msg.sender == owner, "Nice try");
        payable(msg.sender).transfer(address(this).balance);
    }
}
```
