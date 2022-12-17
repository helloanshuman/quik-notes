This repo is to be used to save my quick notes

	const a = service.methodA(); // returning Observable<aResponse>
	
	const b = a.pipe(concatMap(

	  aResponse => {

		//use aResponse

		let bResponse$ = of(null);

		bResponse$ = service.methodB(); // returning Observable<bResponse>

	  }
	));

	this.subs.add(

	  b.subscribe( bResponse => {

		// use bResponse

	  })
	)
