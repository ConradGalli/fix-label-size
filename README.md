fix-label-size
==============
	jQuery('body').on('click', '.print',function(e){
 		e.preventDefault();
 		      var image = jQuery(this).data("imgid");
		      var win = window.open('', 'Image', 'resizable=yes,...');
		      if (win.document) {
				win.document.writeln('<img style="width: 350px;height: 520px;" src="'+ image +'" alt="image" />');
				//win.document.close();
				//win.focus();
				//win.print();
		      }
 	      return false;

	});
