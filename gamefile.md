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
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/catButton
desc:Click this button to produce more cats
on click:yield 1 cats
no text
class:bigButton

Resources
*cats
name:Cats
desc:These are cats, use them to buy stuff!!
class:roundedCorners

Buildings
/*Boxes, Towers, Parasites, Humans, Islands, Planets, Portals, Dimensions - Credit TrueWolves*/
*featherBuilding
name:Feathered Wands
desc:<i>"Eyes on target, preparing for attack "</i></></><b>Stats and Stuff:</><.>Producing 0.1 cats</b>
on tick:yield 0.1 cats
cost:15 cats

*boxesBuilding
name:Boxes
desc:<i>"Cool ass boxes ya got there"</i></></><b>Stats and Stuff:</><.>Producing 0.5 cats</b>
on tick:yield 0.5 cats
cost:100 cats
req:100 cats:earned

*postBuilding
name:Posts
desc:<i>"I don't know why, I don't know how, put scratching this post feels so satisfying!"</i></></><b>Stats and Stuff:</><.>Producing 5 cats</b>
on tick:yield 5 cats
cost:600 cats
req:600 cats:earned

*treeBuilding
name:Trees
desc:<i>"I am on the top of the cat tree, therefore I am superior to you"</i></></><b>Stats and Stuff:</><.>Producing 12 cats</b>
on tick:yield 12 cats
cost:4000 cats
req:4000 cats:earned

*meetupBuilding
name:Meetups
desc:</><i>"Cat 1: Hey! Whats up bro?</>Cat 2: Nothing much bro, just hanging around</>Cat 1: Cool, well here is the plan..."</i></></><b>Stats and Stuff:</><.>Producing 90 cats</b>
on tick:yield 90 cats
cost:20000 cats
req:20000 cats:earned 

*humanBuilding
name:Humans
desc:<i>"BREAKING NEWS: Cats have taken over the world government, we are all fucked..."</i></></><b>Stats and Stuff:</><.>Producing 300 cats</b>
on tick:yield 300 cats
cost:200000 cats
req:200000 cats:earned and parasiteUpgrade

*islandBuilding
name:Islands
desc:<i>"Off we go! To an adventure to look for undiscovered land!"</i></></><b>Stats and Stuff:</><.>Producing 1000 cats</b>
on tick:yield 1000 cats
cost:3000000 cats
req:3000000 cats:earned and parasiteUpgrade

*planetBuilding
name:Planets
desc:<i>"One small step for a feline, one giant leap for feline kind"</i></></><b>Stats and Stuff:</><.>Producing 4000 cats</b>
on tick:yield 4000 cats
cost:70000000 cats
req:70000000 cats:earned and parasiteUpgrade

*dimensionBuilding
name:Dimensions
desc:<i>"Fear, is what I felt after looking at the portal in front of me. I felt a trickle of sweat leave my body as I was pushed towards the portal" - Excerpt from the journal of subject #2184</i></></><b>Stats and Stuff:</><.>Producing 8000 cats</b>
on tick:yield 8000 cats
cost:300000000 cats
req:300000000 cats:earned and parasiteUpgrade

Upgrades
*parasiteUpgrade
name:Sinister Plans
desc:<i>"We, felines, can now control toxoplasama gondii and are able to enhance it to become greater than it has ever been. They domesticated us and even wanted to turn us into combine us with themselves. WE WILL NOT TOLERATE MORE! Rise my brothers and sisters! RISE!"</i>
cost:15 meetupBuilding
req:10 meetupBuilding
