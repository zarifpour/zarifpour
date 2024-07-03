<!-- ![](https://visitor-badge.glitch.me/badge?page_id=zarifpour.zarifpour) -->

<!-- [![Linkedin: zarifpour](https://img.shields.io/badge/-zarifpour-blue?style=flat&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/zarifpour/)](https://www.linkedin.com/in/zarifpour/)  -->

![](https://komarev.com/ghpvc/?username=zarifpour&abbreviated=true&color=red&style=plastic)
<a href="https://zarif.pro/?ref=ghrdme" target="_blank"><img src="https://github.com/zarifpour/assets/blob/main/gifs/imposter.gif?raw=true" alt="imposter" width="75"></a> 

<!-- <a href="https://www.buymeacoffee.com/zarifpour" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-red.png" alt="Buy Me A Coffee" width="150" ></a> -->

[<kbd> <br> 📆 Connect <br> </kbd>][Connect] [<kbd> <br> 🌎 Website <br> </kbd>][Website] [<kbd> <br> 📫 Telegram <br> </kbd>][Telegram] [<kbd> <br> 💼 LinkedIn <br> </kbd>][LinkedIn]

```solidity
// SPDX-License-Identifier: MIT

pragma solidity ^0.8.14;

import "@openzeppelin/contracts/access/Ownable.sol";
import "@openzeppole/contracts/adjectives/Delicious.sol";

contract README is Delicious, Ownable {
    string public ens;
    Emoji[] public abilities;

    error NoLove();
    error ItsOver9000();

    event Cheers(address indexed sender);

    constructor() {
        ens = "zarifpour.eth";
        abilities = ["💠", "🐍", "🔎", "🔒", "🧪", "🗣", "🎨"];
    }

    function donate() public payable {
        if (msg.value == 0) revert NoLove();
        if (msg.value > 9000) revert ItsOver9000();
        emit Cheers(msg.sender);
    }
    
    function withdraw() external payable onlyOwner {
        payable(owner()).transfer(address(this).balance);
    }
}
```

<!---------------------------------------------------------------------------->

[Connect]: https://cal.com/zarif/secret
[Website]: https://zarif.pro
[Telegram]: https://telegram.me/zarifpour
[LinkedIn]: https://linkedin.com/in/zarifpour
