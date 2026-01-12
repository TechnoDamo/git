# What is Git?
It is better to forget all you know of other VCSs when learning Git, because it mey spare you of unnesessary confusion. 

## Snapshots, Not Differences 
The major difference between git and other VCSs is the way Git thinks about its data. <br/>
Conceptually, most other systems store information as a list of files and the changes made to each file over time (*delta-based* version control). <br/>
Git thinks of its data more like a series of snapshopts of a miniature filesystem, like a **stream of snapshots**. If files have not changed, git doesn't store the file again, just a link to the previous identical file it has already stored. 


## Nearly Every Operation Is Local
Most operations in git need only local files and resources to operate because almost all info about the project is stored locally. It is one of the most significant differences from other VCSs where you might quite often need online access use most of the functionality. 

## Git Has Integruty
Git stores all information refering to the SHA-1 checksum of its contents. It means that it is impossible to do any changes to any data within a repo, to lose
information in transit or get file corruption without git knowing it. 
```
24b9da6552252987aa493b52f8696cd6d3b00373
```

## Git Generally Only Adds Data
Nearly all of the actions in Git result with Git only *adding data* to the Git database, so it is hard to do anything undoable after you commit. 

## The Three States

