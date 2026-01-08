Welcome to use the JSON from GitHub, for first use you need this command in VS Code for example or use from GitPage in index:

https://douglasribeirosanguino.github.io/dataTestJson/index

<img width="1533" height="629" alt="image" src="https://github.com/user-attachments/assets/2edf70bb-8267-45b8-936a-066f4ae0436c" />

========= VS Code =========

$data = Invoke-RestMethod https://douglasribeirosanguino.github.io/dataTestJson/dataTestJson.json

this filter below is used only you need infos like a "NUT"
$data.items | Where-Object { $_.name -like "*NUT*" }

But you add texts for more simple read on terminal:

"Status: ", $data.status, "Version: ", $data.version, $data.items

<img width="849" height="695" alt="image" src="https://github.com/user-attachments/assets/b78d9ff9-bf97-4e73-89d1-9c0eb89a94bf" />

