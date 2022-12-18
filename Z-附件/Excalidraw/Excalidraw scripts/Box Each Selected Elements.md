/*
```javascript
*/
const padding = parseInt (await utils.inputPrompt("padding?","number","10"));
elements = ea.getViewSelectedElements();

for(const element of elements) {
	const box = ea.getBoundingBox([element]);
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
	ea.style.strokeStyle = strokeStyle; // NO Working, maybe bug!
	ea.style.roughness = roughness;
	ea.style.fillStyle = fillStyle;
	ea.style.backgroundColor = backgroundColor;
	//uncomment for random color:
	//color = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
	ea.style.strokeColor = color;
	ea.deleteViewElements([element]); // jcl added: First remove the selected object, and then through copyViewElementsToEAforEditing () to add back, this new box will remain below the selected object 
	id = ea.addRect(
		box.topX - padding,
		box.topY - padding,
		box.width + 2*padding,
		box.height + 2*padding
	);
    ea.elementsDict[id].strokeStyle=strokeStyle; // jcl added: ea.elementsDict[id] has no strokeStyle but storkeStyle
	ea.copyViewElementsToEAforEditing([element]);
	ea.addToGroup([id].concat(element.id));
	ea.addElementsToView(false);
}