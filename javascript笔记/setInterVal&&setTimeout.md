###setInterVal

	(function(){
		var	index = 0;
		setInterval(function(){
		var started = new Date(),
				i = index;
	
				index++;
	
				console.log("req "+i+'started at'+started);
	
		}, 3000);
	})();


###setTimeout

	(function(){
		var index = 0;
		setTimeout(function Test(){
			var started = new Date(),
			i = index;
	
			index++;
	
			console.log("req "+i+'started at'+started);
	
			setTimeout(Test, 3000);
		}, 3000);
	})();
	