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
/*Boxes, Towers, Parasites, Humans, Islands, Portals, Planets, Dimensions - Credit TrueWolves*/
*boxesBuilding
name:Box|Boxes
desc:<i>"Cool ass boxes ya got there"</i>
on tick:yield 1 cats
cost:100 cats

*towersBuilding
name:Tower|Towers
desc:<i>"I dunno why, I dunno how, put scratching this post feels so satisfying!"</i>
on tick:yield 5 cats
cost:500 cats

*parasitesBuilding
name:Parasite|Parasites
desc:<i></>"Cat 1: What the fuck did you eat bro?</>Cat 2: I don't know man, tasted kinda funny tho"</i>
on tick:yield 10 cats
cost:1000 cats

*humansBuilding
name:Human|Humans
desc:<i>"BREAKING NEWS: Cats have taken over the world government, we are all fucked..."</i>
on tick:yield 15 cats
cost:1500 cats

*islandBuilding
name:Island|Islands
desc:<i>"We, will for the most part sail until we essentially find fairly more land for our feline specie"</i>
on tick:yield 20 cats
cost:2000 cats

*portalBuilding
name:Portal|Portals
desc:<i>Fear, is what I felt after looking at the portal in front of me. Being a test subject after being enslaved traumatized me. I felt a trickle of sweat leave my body as I was pushed towards the portal" - Excerpt from the journal of subject #2184</i>
on tick:yield 25 cats
cost:2500 cats

*planetBuilding
name:Planet|Planets
desc:<i>One small step for a feline, one giant leap for feline kind</i>
on tick:yield 30 cats
cost:3000 cats

*dimensionBuilding
name:Dimension|Dimensions
desc:<i>We did it, I have entered dimension Dime-420</i>
on tick:yield 35 cats
cost:3500 cats
