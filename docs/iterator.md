## Iterações com array simulando for

var myArray = ['item1','item2','item3'];

	//jQuery
	$.each(myArray, function(index, obj){
		console.log(index, obj);
	});

	//Javascript puro
	for(var x=0, length = myArray.length; x<length; x++){
		console.log(x, myArray[x]);
	}

	// IE9+ (Não suportado no PhantomJS)
	myArray.forEach(function(obj, index){
		console.log(index, obj);
	});

	// IE9+ (Não suportado no PhantomJS)
	Array.prototype.map.call(myArray, function(obj, index) {
		console.log(index, obj);
	});
