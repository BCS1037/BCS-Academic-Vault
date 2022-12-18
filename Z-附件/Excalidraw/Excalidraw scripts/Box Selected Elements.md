/*

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-download-raw.jpg)

Download this file and save to your Obsidian Vault including the first line, or open it in "Raw" and copy the entire contents to Obsidian.

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-box-elements.jpg)

This script will add an encapsulating box around the currently selected elements in Excalidraw.

See documentation for more details:
https://zsviczian.github.io/obsidian-excalidraw-plugin/ExcalidrawScriptsEngine.html

```javascript
*/
//uncomment if you want a prompt for custom padding

const padding = parseInt (await utils.inputPrompt("padding?","number","10"));
//const padding = 10
elements = ea.getViewSelectedElements();
const box = ea.getBoundingBox(elements);
color = ea
        .getExcalidrawAPI()
        .getAppState()
        .currentItemStrokeColor;
// jcl added: use current stroke with and style
strokeWidth = ea.getExcalidrawAPI().getAppState().currentItemStrokeWidth;
strokeStyle = ea.getExcalidrawAPI().getAppState().currentItemStrokeStyle;
roughness = ea.getExcalidrawAPI().getAppState().currentItemRoughness;
fillStyle = ea.getExcalidrawAPI().getAppState().currentItemFillStyle;
backgroundColor = ea.getExcalidrawAPI().getAppState().currentItemBackgroundColor;
ea.style.strokeWidth = strokeWidth;
ea.style.strokeStyle=strokeStyle; // NO Working
ea.style.roughness = roughness;
ea.style.fillStyle = fillStyle;
ea.style.backgroundColor = backgroundColor;
//uncomment for random color:
//color = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
ea.style.strokeColor = color;
ea.deleteViewElements(elements); // jcl added: First remove the selected object, and then through copyViewElementsToEAforEditing () to add back, this new box will remain below the selected object 
id = ea.addRect(
	box.topX - padding,
	box.topY - padding,
	box.width + 2*padding,
	box.height + 2*padding
);
ea.elementsDict[id].strokeStyle=strokeStyle; // jcl added: ea.elementsDict[id] has no strokeStyle but storkeStyle
ea.copyViewElementsToEAforEditing(elements);
ea.addToGroup([id].concat(elements.map((el)=>el.id)));
ea.addElementsToView(false);
