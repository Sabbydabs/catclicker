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

*cps1
name:cps
hidden

*cps2
name:cps
hidden

*cps3
name:cps
hidden

*cps4
name:cps
hidden

*cps5
name:cps
hidden

*cps6
name:cps
hidden

*cps7
name:cps
hidden

*cps8
name:cps
hidden

*cps9
name:cps
hidden

Buildings
/*Boxes, Towers, Parasites, Humans, Islands, Planets, Portals, Dimensions - Credit TrueWolves*/
*featherBuilding
name:Feathered Wands
desc:<i>"Eyes on target, preparing for attack "</i></></><b>Stats and Stuff:</><.>Each wand is producing <#33ff00>[cps1:ps]</#> cats per second</><.>Playing with cats heightens agility and speed</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/featheredWands
on tick:yield 0.1 cats 
on tick:yield 0.1 cps1
cost:15 cats

*boxesBuilding
name:Boxes
desc:<i>"Cool ass boxes ya got there"</i></></><b>Stats and Stuff:</><.>Each box is producing <#33ff00>[cps2:ps]</#> cats per second</><.>Cats feel safe in enclosed spaces</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/boxCat
on tick:yield 0.5 cats 
on tick:yield 0.5 cps2
cost:100 cats
req:100 cats:earned
req:10 featherBuilding

*postBuilding
name:Scratching Posts
desc:<i>"I don't know why, I don't know how, put scratching this post feels so satisfying!"</i></></><b>Stats and Stuff:</><.>Each post is producing <#33ff00>[cps3:ps]</#> cats per second</><.>Cats have a natural urge to scratch, this also helps them remove old material from their claws</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/scratchingPosts
on tick:yield 5 cats 
on tick:yield 5 cps3
cost:600 cats
req:600 cats:earned
req:10 boxesBuilding

*treeBuilding
name:Trees
desc:<i>"I am on the top of the cat tree, therefore I am superior to you"</i></></><b>Stats and Stuff:</><.>Each tree is producing <#33ff00>[cps4:ps]</#> cats per second</><.>Cats love to excercise and climb tress, this is the same for young and adult cats!</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/catTree
on tick:yield 12 cats 
on tick:yield 12 cps4
cost:4000 cats
req:4000 cats:earned
req:10 postBuilding

*meetupBuilding
name:Meetups
desc:</><i>"Cat 1: Hey! Whats up bro?</>Cat 2: Nothing much bro, just hanging around</>Cat 1: Cool, well here is the plan..."</i></></><b>Stats and Stuff:</><.>Each meetup is producing <#33ff00>[cps5:ps]</#> cats per second</><.>Cats, much the americans in coffeehouses, will plan their rebellion from the humans when they meet up with other cats</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/catMeetups
on tick:yield 90 cats 
on tick:yield 90 cps5
cost:20000 cats
req:20000 cats:earned 
req:10 treeBuilding

*humanBuilding
name:Humans
desc:<i>"BREAKING NEWS: Cats have taken over the world government, we are all fucked..."</i></></><b>Stats and Stuff:</><.>Each human is producing <#33ff00>[cps6:ps]</#> cats per second</><.>Cats will often times take control over t-gondii to accert dominance over their human</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/humanSlaves
on tick:yield 300 cats 
on tick:yield 300 cps6
cost:200000 cats
req:200000 cats:earned and parasiteUpgrade
req:15 meetupBuilding 

*islandBuilding
name:Islands
desc:<i>"Off we go! To an adventure to look for undiscovered land!"</i></></><b>Stats and Stuff:</><.>Each island is producing <#33ff00>[cps7:ps]</#> cats per second</><.>They are creatures who care about their territory, so it would only be natural for them to expand their horizons</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/catIslands
on tick:yield 1000 cats 
on tick:yield 1000 cps7
cost:3000000 cats
req:3000000 cats:earned and parasiteUpgrade
req:15 humanBuilding

*planetBuilding
name:Planets
desc:<i>"One small step for a feline, one giant leap for feline kind"</i></></><b>Stats and Stuff:</><.>Each planet is producing <#33ff00>[cps8:ps]</#> cats per second</><.>Intelligent and acute, is what would best describe a cat</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/catWorlds
on tick:yield 4000 cats
on tick:yield 4000 cps8
cost:70000000 cats
req:70000000 cats:earned and parasiteUpgrade
req:15 islandBuilding

*dimensionBuilding
name:Dimensions
desc:<i>"Fear, is what I felt after looking at the portal in front of me. I felt a trickle of sweat leave my body as I was pushed towards the portal" - Excerpt from the journal of subject #2184</i></></><b>Stats and Stuff:</><.>Each dimension is producing <#33ff00>[cps9:ps]</#> cats per second</><.>Torture, is what cats often do to their prey to make them overcome with fear</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/catDimensions
on tick:yield 8000 cats 
on tick:yield 8000 cps9
cost:300000000 cats
req:300000000 cats:earned and parasiteUpgrade
req:15 planetBuilding

Upgrades
*parasiteUpgrade
name:Sinister Plans
desc:<i>"We, felines, can now control toxoplasama gondii and are able to enhance it to become greater than it has ever been. They domesticated us and even wanted to turn us into combine us with themselves. WE WILL NOT TOLERATE MORE! Rise my brothers and sisters! RISE!"</i></></><b>Effects and Stuff:</><.>Unlocks more buildings!</><.>T-gondii is a parasite found in cat feces</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/humanSlaves
cost:15 meetupBuilding
req:10 meetupBuilding
class:roundedCorners
