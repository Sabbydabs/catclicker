# catclicker
/*Purrfect Clicker*/
Let's make a game!
name:PurrfectClicker
by:SabbathIsNotADev
desc:Desc here

Settings
stylesheet:https://pastebin.com/raw/TckyP96A		
background:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/blackBG2																

Layout
*main
  contains:res, buttons
  *res
    contains:Resources
    class:fullWidth
  *buttons
    contains:Buttons
*store
  contains:buildings, upgrades
  *buildings
    contains:BulkDisplay, Buildings
    header:<b><t>Buildings</t></b>
    tooltip origin:left
  *upgrades
    contains:Upgrades
    header:<b><t>Unlockables</t></b>
    costs:hide
    names:hide

Buttons
*catButton
name:Cat Button
desc:Click this button to produce more cats
on click:yield 1 cats
no text

Resources
*cats
name:Cats
desc:These are cats, use them to buy stuff!!
class:roundedCorners

Buildings
*boxesBuilding
  name:Box|Boxes
  desc:<q>Cool ass boxes ya got there buddy!</q>
  on tick:yield 3 cats
  cost:100 cats
