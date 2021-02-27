/*Purrfect Clicker - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - */
/*https://www.desmos.com/calculator/eun6ycoojl*/
Let's make a game!
name:Catastrophik
by:SabbathIsNotADev
desc:Desc here
 
Settings
stylesheet:https://pastebin.com/raw/TckyP96A
background:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/blackBG2		
building cost increase:125%														
 
Layout
*main
  contains:res, buttons
  *res
    contains:Resources
    class:resPosition fullWidth
  *buttons
    contains:Buttons
*store
  contains:buildings, upgrades, ownedupgrades, ownedachievs
  *buildings
    contains:BulkDisplay, Buildings
    header:<b><t>Buildings</t></b>
    tooltip origin:left
  *ownedachievs
	contains:Achievements
	header:<b><t>Achievements</t></b>
	costs:hide
	names:hide
  *upgrades
    contains:Upgrades
    header:<b><t>Upgrades</t></b>
    costs:hide
    names:hide    
  *ownedupgrades
    contains:tag:owned
    header:<b><t>Owned Upgrades</t></b>
    costs:hide
    names:hide
	class:ownedUpgrades
	
*log
    contains:Log
    class:bottom
 
Buttons
*catButton
name:Big Cat
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/catButton
desc:Click this button to produce more cats
on click:yield 1 cats
on click:if (have click2) yield 1 cat2
on click:if (have click3) yield 1 cat3
on click:if (have click4) yield 1 cat4
on click:if (have click5) yield 1 cat5
on click:if (have click6) yield 1 cat6
on click:if (have click7) yield 1 cat7
on click:if (have click8) yield 1 cat8
on click:if (have click9) yield 1 cat9
no text
class:bigButton
on load:log <t><u>Change-Log</u></t><//></><t>Random Something #1<//><.>I really don't know how I am physicaly tired by just setting this log up...<.>Game still in beta
 
on start:log <t><u>Change-Log</u></t><//></><t>Random Something #1<//><.>I really don't know how I am physicaly tired by just setting this log up...<.>Game still in beta

*gameTitle
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/Catastrophik
on click:anim icon wobble
class:gameTitle
icon class:titleIcon
no text
no tooltip

*creditsCat
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/creditsCat
class:creditsCat meta-button
icon class:creditsIcon
no text
name:Credits
desc:Nothing, game still unfinished...

Resources
*cats
name:Cats
desc:These are cats, use them to buy stuff!!
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click1
class:resPosition
 
*cat2
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click2
hidden
 
*cat3
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click3
hidden
 
*cat4
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click4
hidden
 
*cat5
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click5
hidden
 
*cat6
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click6
hidden
 
*cat7
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click7
hidden
 
*cat8
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click8
hidden
 
*cat9
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click9
hidden
 
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
*TEMPLATE
class:roundedCorners

/*----------------------------------------------------------------------------------------------------------*/

*parasiteUpgrade
name:Sinister Plans
desc:<i>"We, felines, can now control toxoplasama gondii and are able to enhance it to become greater than it has ever been. They domesticated us and even wanted to turn us into combine us with themselves. WE WILL NOT TOLERATE MORE! Rise my brothers and sisters! RISE!"</i></></><b>Effects and Stuff:</><.>Unlocks more buildings!</><.>T-gondii is a parasite found in cat feces</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/humanSlaves
cost:15 meetupBuilding
req:10 meetupBuilding
class:roundedCorners
 
/*button Upgrades - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
**Tempelate:**
*click
name:
desc:<i>""</i></></><b>Effects and Stuff:</><.>Doubles the yield of the big cat</b>
icon:
passive:multiply yield of catButton by 1
cost:
req:
class:roundedCorners
*/
 
*click1
name:Basic Cats
desc:<i>"A basic cat, not much"</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 1</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click1
passive:increase yield of catButton by 1
cost:100 cats
req:1 cats:earned
 
*click2
name:Purple Cats
desc:<i>"Now this is just ridiculous! A purple cat? The creator is running out of ideas ALREADY?!?? Geez, so uncreative..."</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 1</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click2
passive:increase yield of catButton by 1
cost:200 cats
req:50 cats:earned
req:1 click1
 
*click3
name:Jade Cats
desc:<i>"Cats can finally express themselves and can show their true colors.. <b>literally</b>"</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 2</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click3
passive:increase yield of catButton by 2
cost:400 cats
req:1 click2
req:200 cats:earned
 
*click4
name:Auric Cats
desc:<i>"Golden and shimmering with stellar beauty"</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 2</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click4
passive:increase yield of catButton by 2
cost:3000 cats
req:1 click3
req:1000 cats:earned
 
*click5
name:Scarlet Cats
desc:<i>"Rumors has it that they only appear on a blood moon!"</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 2</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click5
passive:increase yield of catButton by 2
cost:10000 cats
req:1 click4
req:1000 cats:earned
 
*click6
name:Earthly Cats
desc:<i>"Flora and Fauna, they love it all!"</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 2</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click6
passive:increase yield of catButton by 2
cost:50000 cats
req:1 click5
req:10000 cats:earned
 
*click7
name:Violaceous Cats
desc:<i>"Inky cats..."</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 2</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click7
passive:increase yield of catButton by 2
cost:100000 cats
req:1 click6
req:50000 cats:earned
 
*click8
name:Ivy Cats
desc:<i>"Their claws reek with poison, one strike from these and ya can kiss ya ass goodbye!"</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 2</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click8
passive:increase yield of catButton by 2
cost:500000 cats
req:1 click7
req:100000 cats:earned
 
*click9
name:Citric Cat
desc:<i>"Full of energy and swift as can be!"</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 2</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click9
passive:increase yield of catButton by 2
cost:1000000 cats
req:1 click8
req:500000 cats:earned

*click10 
name:Recycling Cats
desc:<i>"Reduce, Re-use, Recycle is there motto, and it should be yours too! ;)"</i></></><b>Effects and Stuff:</><.>Increases the yield of the big cat by 2</b>
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click10
passive:increase yield of catButton by 2
cost:10000000 cats
req:1000000 cats:earned
 
/*building upgrades - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -*/
/*
*buildingUpgrade1
name:Sparkles
desc:<i>"Oooh, Sparkly!"</i></></><b>Effects and Stuff:</><.>Duplicates the production of feathered wands, boxes and scratching posts</b>
icon:
cost:1000 cats
passive:multiply yield of featherBuilding by 2
passive:multiply yield of boxesBuilding by 2
passive:multiply yield of postBuilding by 2
req:(featherBuilding>=10 or boxesBuilding>=10 or postBuilding>=10)

*buildingUpgrade2
name:Scents
desc:<i>"The scent of this toy is delicious"</i></></><b>Effects and Stuff:</><.>Duplicates the production of feathered wands, boxes and screathing posts</b>
icon:
cost:100000 cats
passive:multiply yield of featherBuilding by 2
passive:multiply yield of boxesBuilding by 2
passive:multiply yield of postBuilding by 2
req:(featherBuilding>=50 or boxesBuilding>=50 or postBuilding>=50)

*buildingUpgrade3
name:Quality Material
desc:<i>"Quality material, forever and ever"</i></></><b>Effects and Stuff:</><.>Duplicates the production of feathered wands, boxes and scratching posts</b>
icon:
cost:5000000 cats
passive:multiply yield of featherBuilding by 2
passive:multiply yield of boxesBuilding by 2
passive:multiply yield of postBuilding by 2
req:(featherBuilding>=100 or boxesBuilding>=100 or postBuilding>=100)

*buildingUpgrade4
name:Better Hiding Spots
desc:<i>"These hiding sport are wickedly rad!"</i></></><b>Effects and Stuff:</><.>Duplicates the production of trees and meetups</b>
icon:
cost:50000 cats
passive:multiply yield of treeBuilding by 2
passive:multiply yield of meetupBuilding by 2
req:(treeBuilding>=10 or meetupBuilding>=10)

*buildingUpgrade5
name:Taller Trees
desc:<i>"These taller trees will help us keep our meetings more secret"</i></></><b>Effects and Stuff:</><.>Duplicates the production of trees and meetups</b>
icon:
cost:5000000 bunnies
passive:multiply yield of treeBuilding by 2
passive:multiply yield of meetupBuilding by 2
req:(treeBuilding>=50 or meetupBuiliding>=50)

*buildingUpgrade6
name:Better Boats
desc:<i>"To ensure the health of humans we need to create better boats! Sick humans won't work!"</i></></><b>Effects and Stuff:</><.>Duplicates the production of humans and islands</b>
icon:
cost:1000000 cats
passive:multiply yield of humanBuilding by 2
passive:multiply yield of islandBuilding by 2
req:(humanBuilding>=10 or islandBuilding>=10)

*buildingUpgrade7
name:Human Food
desc:<i>"Most, have noticed that humans don't like cat food, so we shall prepare them filthy human food instead"</i></></><b>Effects and Stuff:</><.>Duplicates the production of humans and islands</b>
icon:
cost:500000000 cats
passive:multiply yield of humanBuilding by 2
passive:multiply yield of islandBuilding by 2
req:(humanBuilding>=50 or islandBuilding>=50)

*buildingUpgrade8
name:Enhanced Spaceships
desc:<i>"In order to ensure the safety of cats and slaves we need to enhance the rusty, old and cheap human spaceships"</i></></><b>Effects and Stuff:</><.>Duplicates the production of </b>
icon:
cost:1000000000 cats
passive:multiply yield of planetBuilding by 2
passive:multiply yield of dimensionBuilding by 2
req:(planetBuidling>=10 or dimensionBuilding>=10)

/*
*buildingUpgrade
name:
desc:<i>""</i></></><b>Effects and Stuff:</><.>Duplicates the production of </b>
icon:
cost:
passive:
passive:
passive:
req:

*buildingUpgrade
name:
desc:<i>""</i></></><b>Effects and Stuff:</><.>Duplicates the production of </b>
icon:
cost:
passive:
passive:
passive:
req:

*buildingUpgrade
name:
desc:<i>""</i></></><b>Effects and Stuff:</><.>Duplicates the production of </b>
icon:
cost:
passive:
passive:
passive:
req:


*/

Achievements
*TEMPLATE
class:roundedCorners
/*----------------------------------------------------------------------------------------------------------*/

*testAchiev
name:Test
desc:test
req:1 cats
icon:https://pipe.miroware.io/5f91b0d7e6bde66c95ca308c/click1
