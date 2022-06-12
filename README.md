# Dofus Quest Graph

### Introduction

Every now and then, whenever new server comes up, we want to create a new main or we're coming to some content we haven't approached before, we usually rely on dofuspourlesnoobs, dofuswiki or some other pages to help us see where to go and what to do.

Sometimes though we do encounter a questline that requires another questline that requires another questline that requires something else again.

There is also another thing of one dungeon appearing in different questlines, e.g. key master's smith dungeon will come up in bonta's alignment quest. Nileza comes up two or three times in Ice dofus quest.

So I thought, how nice it would be to have it visualized and described.

Therefore, I am looking for people that would like to contribute to such a project in GraphViz.

My discord tag is Jenuzor#7117, pm me if you're up!

If you have any additional comments or suggestions, feel free to put them in!


### How to use it

Copy-paste the contents of graph.pv into a GraphViz engine, like edotor.net .

This should show you what it looks like.


### How to contribute

Try to edit the graph.gv file, and then submit that in a PR.

We want to create more ``` subgraphs ``` that show different quests and then link them to the dungeons.

Dungeons will be a separate subgraph on it's own.

The colouring, shapes, linking is not decided yet.

So far, the template for a new quest/questline is
```
subgraph "{questline name}" {
  {unique ID} [label="{quest name or step name}"];
  {unique ID} [label="{quest name or step name}"];
  {unique ID} [label="{quest name or step name}"];
}
```

Please try to put the IDs below one another, so that the last questline subgraph has the highest ID.


### TODO

- All dungeons and quests
- A decision on colouring and shaping. We can use different shapes like box/ellipse/circle/rhombus, as well as different colors for the borders/background/links to depict the relation, e.g. red line between nodes means that the step ends the quest, blue line between nodes is a dungeon-quest link, golden line is for achievements etc.
- Find a way of how to position them together, so they would be more readable in the longer term. Maybe put the dungeons in a straight line and then other quest lines would just go in parallel, rather than make them float around one another?
