## Iterações com array simulando for

	var myArray = ['item1', 'item2', 'item3'];
	
	//jQuery
	$.each(myArray, function(index, obj){
		console.log(index, obj);
	});
	
	//Javascript puro
	for(var i = 0, len = myArray.length; i < len; i++){
		console.log(i, myArray[i]);
	}
	
	myArray.forEach(function(obj, index){
		console.log(index, obj);
	});
