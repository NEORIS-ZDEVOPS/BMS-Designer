# Index
- [Index](#index)
- [Introduction](#introduction)
	- [Open the TreeView](#open-the-treeview)
	- [Tabs view](#tabs-view)
	- [Deploy nodes](#deploy-nodes)
	- [Comments](#comments)
	- [Node Actions](#node-actions)
	- [File node](#file-node)
	- [DFHPSD node](#dfhpsd-node)
	- [DFHPDI node](#dfhpdi-node)
	- [DFHMSD node](#dfhmsd-node)
	- [DFHMDI node](#dfhmdi-node)
	- [DFHMDF node](#dfhmdf-node)

# Introduction

The extension adds a tree view for the BMS hierachy that enables multiple actions.

## Open the TreeView <a id="open-the-treeview"></a>

![gif featuring TreeView](./assets/TreeView.gif)

Prerequisite: Having a .bms opened.

1. Click on the "Explorer" tab in the Sidebar
2. The "MY TREE VIEW" container will display the hierarchical tree

## Tabs view <a id="tabs-view"></a>

![gif featuring tabs view](./assets/TabsView.gif)

1. Click on the "Source" tab to switch to source mode if the view remains in design mode.
2. Click on the "Design" tab to switch to design mode if the view remains in source mode.

## Deploy nodes <a id="deploy-nodes"></a>

![gif featuring Deploy nodes](./assets/DeployNodes.gif)

Prerequisite: The node must have children in order to be deployed.

1. Click on the node to deploy its child nodes.
2. Click again on the parent node to collapse the child nodes.

## Comments <a id="comments"></a>

![gif featuring comments](./assets/Comment.gif)

1. Right-click on the node(except file node) and click "Add comment"
2. Enter the comment in the QuickPick menu

Notes:
1. If a node has comment(s), a "(c)" will apear to it's right
2. To view the comments in design mode, place the cursor on a node, the comments will apear in an emergent menu
3. In the source mode, the commens  will be placed above the selected node.
4. When adding a map set or a partition set to a file, a header comment will be included, providing information about the date and extension.

![png featuring header](./assets/header.png)

## Node Actions <a id="node-actions"></a>

![gif featuring node actions](./assets/NodeActions.gif)


Info: For each node, we will have specific actions corresponding to the functionality associated with each macro.

1. Click righ buttom on the node to display the menu.
2. Double-click on the node to edit the macro. (File nodes do not have this feature.).To learn more about this feature, refer to the   [Edit macro section](designview.MD/#edit-macro)


Note:The double-click feature in source mode will place the cursor on that macro.

![gif featuring node actions](./assets/NodeActionsDblClick.gif)

## File node <a id="file-node"></a>

The file node is represented by this icon: 
![png featuring node ](./assets/FileNode.png)

The file node actions are as follows:

- Add map set

![gif featuring add map set](./assets/AddMapSet.gif)

1. Click right buttom on the node and select "Add map set"
2. If the view design mode is selected, we have to introduce a valid name for the map set .

Notes:
1. If a map set already exists, it will prevent the addition of a new one.
2. Add a map with same name.

- Add partition set

![gif featuring add partition set](./assets/AddPartitionSet.gif)

1. Click right buttom on the node and select "Add partition set"
2. If the view design mode is selected, we have to introduce a valid name for the partition set.

Note: If a partition set already exists, it will prevent the addition of a new one.

## DFHPSD node <a id="dfhpsd-node"></a>
The dfhpsd node is represented by this icon:
![png featuring partition set ](./assets/PartitionSet.png)

The dfhpsd node actions are as follows:

- Edit macro

![gif featuring edition macro ](./assets/EditMacro.gif)

1. Click right buttom on the node and select "Edit macro"

Note: 
1. This feature is common for all nodes (except the file node) and functions the same as double-clicking on the node.

- Delete partition set
![gif featuring delete partition set ](./assets/DeletePartitionSet.gif)

1. Click right buttom on the node and select "Delete partition set"

Note:
1. As a hierarchical type, all the child nodes (dfhpdi, comments) will also be deleted.
2. If a map set does not exist, the header will also be deleted along with the partition set

## DFHPDI node <a id="dfhpdi-node"></a>
The dfhpdi node is represented by:
![png featuring partition  ](./assets/partition.png)

The dfhpdi node actions are as follows:

-Delete partition
![gif featuring delete partition ](./assets/DeletePartition.gif)

1. Click right buttom on the node and select "Delete partition"

Note:
1. When you add a partition to a partition set, it will be placed between the partition sets, as can be observed in the source mode.


## DFHMSD node <a id="dfhmsd-node"></a>

The dfhmsd node is represented by this icon:
![png featuring map set  ](./assets/maspset.png)

The dfhmsd node actions are as follow

- Add map
![gif featuring add map ](./assets/AddMap.gif)

1. Click right buttom on the node and select "Add map"
2. Introduce a name for the map in the QuickPick menu and press enter to accept

Notes:
1. Similar to partitions, maps will also be included in the source mode between the map set.
2. In design mode, the 'No maps in file' message will disappear once a map is included
3. Multiple maps can be addded to a map set.

- Delete map set
![gif featuring delete map set ](./assets/DeleteMapSet.gif)

1. Click right buttom on the node and select "Delete map set".

Notes:
1. As a hierarchical type, all the child nodes (dfhmdi,dfhmdf comments) will also be deleted.
2. If a partition set does not exist, the header will also be deleted along with the map set

## DFHMDI node <a id="dfhmdi-node"></a>

The dfhmdi node is represented by this icon:
![png featuring map ](./assets/map.png)

Notes:
1. The DFHMDF macros, has different structures that are defined by their attributes. Additionally, some of these fields create a special field with the 'askip' attribute, which cannot be modified but can be moved or deleted using the special field next to which it has been created.



The DFHMDF macro with "askip" atribute is represented by this icon:
![png featuring askip ](./assets/askip.png)

The dfhmdi node actions are as follow


- Add Label
![gif featuring add label ](./assets/AddLabel.gif)

1. Click right on the map buttom and select "Add label field"
2. Introduce a name for the label in the QuickPick menu and press enter to accept.

Note:
1. The label field doesn't create a special 'askip' field with it

- Add Input
![gif featuring add input ](./assets/AddInput.gif)

1. Click right on the map buttom and select "Add input field"
2. Introduce a name for the input in the QuickPick menu and press enter to accept.

Note:
1. The input field create a special 'askip' field with it

-  Add numeric field
![gif featuring add numeric ](./assets/AddNumeric.gif)

1. Click right on the map buttom and select "Add numeric field"
2. Introduce a name for the numeric in the QuickPick menu and press enter to accept.

Note:
1. The numeric field create a special 'askip' field with it


- Add password field
![gif featuring add numeric ](./assets/AddPassword.gif)

1. Click right on the map buttom and select "Add password field"
2. Introduce a name for the password in the QuickPick menu and press enter to accept.

Note:
1. The password field create a special 'askip' field with it

- Add message field
![gif featuring add message ](./assets/AddMessage.gif)

1. Click right on the map buttom and select "Add message field"
2. Introduce a name for the message in the QuickPick menu and press enter to accept.

Note:
1. The label message doesn't create a special 'askip' field with it

- Add output field
![gif featuring add message ](./assets/AddOutPut.gif)

1. Click right on the map buttom and select "Add output field"
2. Introduce a name for the output in the QuickPick menu and press enter to accept.

Note:
1. The label output doesn't create a special 'askip' field with it


- Delete map
![gif featuring delete map ](./assets/DeleteMap.gif)

1. Click right on the node buttom and select "Delete map"

Note:
1. As a hierarchical type, all the child nodes (dfhmdf comments) will also be deleted

## DFHMDF node <a id="dfhmdf-node"></a>
The dfhmdi node is represented by this icon:
![png featuring field ](./assets/field.png)

The dfhmdi node actions are as follow

- Delete a DFHMDF macro with another DFHMDF macro with 'askip'

Note:
1. If the DFHMDF macro creates another field with "askip" atribute, it will also be deleted 

![gif featuring delete field with askip ](./assets/DeleteAskip.gif)

1. Click right on the node buttom and select "Delete field"

 - Delete a DFHMDF macro without another DFHMDF macro with 'askip'

![gif featuring delete field with askip ](./assets/DeleteField.gif)

- 
