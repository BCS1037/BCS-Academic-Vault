/*
set relations between two entities

promp to set description of relation

by noteBeliever

2022/3/22 下午7:04


```javascript
*/

if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.5.21")) {
  new Notice("This script requires a newer version of Excalidraw. Please install the latest version.");
  return;
}

settings = ea.getScriptSettings();
//set default values on first run
if(!settings["Starting arrowhead"]) {
	settings = {
	  "Starting arrowhead" : {
			value: "none",
      valueset: ["none","arrow","triangle","bar","dot"]
		},
		"Ending arrowhead" : {
			value: "triangle",
      valueset: ["none","arrow","triangle","bar","dot"]
		},
		"Line points" : {
			value: 1,
      description: "Number of line points between start and end"
		}
	};
	ea.setScriptSettings(settings);
}

const arrowStart = settings["Starting arrowhead"].value === "none" ? null : settings["Starting arrowhead"].value;
const arrowEnd = settings["Ending arrowhead"].value === "none" ? null : settings["Ending arrowhead"].value;
const linePoints = Math.floor(settings["Line points"].value);


const elements = ea.getViewSelectedElements();
ea.copyViewElementsToEAforEditing(elements);
groups = ea.getMaximumGroups(elements);
if(groups.length !== 2) {
  //unfortunately getMaxGroups returns duplicated resultset for sticky notes
  //needs additional filtering
  cleanGroups=[];
  idList = [];
  for (group of groups) {
    keep = true;
    for(item of group) if(idList.contains(item.id)) keep = false;
    if(keep) {
      cleanGroups.push(group);
      idList = idList.concat(group.map(el=>el.id))
    }
  }
  if(cleanGroups.length !== 2) return;
  groups = cleanGroups;
}
els = [ 
  ea.getLargestElement(groups[0]),
  ea.getLargestElement(groups[1])
];

ea.style.strokeColor = els[0].strokeColor;
ea.style.strokeWidth = els[0].strokeWidth;
ea.style.strokeStyle = els[0].strokeStyle;
ea.style.strokeSharpness = els[0].strokeSharpness;

// insert a letter

// prompt to get string
let let_str = "is";
let_str = await utils.inputPrompt("relation is?","string",let_str);

// set pos of letter in middle
x_letter = (els[0].x + els[1].x ) * 0.5;
y_letter = (els[0].y + els[1].y ) * 0.5;

n_letter = ea.addText(x_letter,y_letter,let_str);

// connect in middle

ea.connectObjects(
  els[0].id,
  null,
  n_letter,
  null, 
  {
	endArrowHead: arrowStart,
	startArrowHead: arrowStart, 
	numberOfPoints: linePoints
  }
);

ea.connectObjects(
  n_letter,
  null,
  els[1].id,
  null, 
  {
	endArrowHead: arrowStart,         // no arrow
	startArrowHead: arrowStart, 
	numberOfPoints: linePoints
  }
);


ea.addElementsToView(false,false,true);
