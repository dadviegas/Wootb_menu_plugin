Web out of the box jquery Menu Plugin

In this example json is used to add the menu items dynamically.

It uses two plugins wootb.menu.js and wootb.corner.js, wootb.menu.js depends of wootb.corner.js.

In wootb.menu.js the click event is passed to the plugin, the action of the click is handled by you.

function dynamicLoadPage(event)
	{
		var $this = $(event.data.element);
		alert($this.attr('rel'));
	}
	
$("#element").menu({paddingDirection:'Left',clickEvent:dynamicLoadPage});